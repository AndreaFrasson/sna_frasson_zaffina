# Data_Collection Phase <br>
Inside this directory all the files used to create the dataset and the graph can be found. <br>
To avoid duplicate (or nearly duplicate) files, we decided to keep one file for explain how we retrieved data from the italian db. More information on 'https://dati.camera.it/sparql'. <br>
To query the db, the schema is reported in the file <i>query_db.ipynb</i>, where is showed how we retrieved monthly data, but simple modifications to the code allowed us to extract data for different temporal windows, for example annual data, quarterly data or aggregated in a more specific way to data extract data for a whole legislation.<br>
The same can be applied to the extraction and construction of the graphs (and relative files). We leave all details about the building phase of the networks in the report, and use the <i>preprocess.ipynb</i> file to explain our working flow from the .csv file to a final graph.


The preprocessing done to the data is better described in the report.
We map voting expressions into integers following this criteria:
- Favorevole = 1
- Contrario = 3
- Astensione = 4
- Assente/Non Ha votato/In missione = 0
