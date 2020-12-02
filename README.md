# API_ETL_Assignment

This API project aims for building a ETL pipeline where API is a primarily method to get the source data. Since we are usually dealing with different kind of data and its sources. 
Three publicly avaialbe  data sources are used. The following is their information:
1. Pollution Data: “https://api.openaq.org/v1/latest?country=IN&limit=10000" .
2. Economy Data: “https://api.data.gov.in/resource/07d49df4-233f-4898-92db-e6855d4dd94c?api-key=579b464db66ec23bdd000001cdd3946e44ce4aad7209ff7b23ac571b&format=json&offset=0&limit=100"
3. Crypto Currencies: https://raw.githubusercontent.com/diljeet1994/Python_Tutorials/master/Projects/Advanced%20ETL/crypto-markets.csv
Please notice that the first two data sets are in json format and the last one is in csv format.

extract.py
Since we are using APIS and CSV file only as our data source, so we will create two generic functions 
that will handle API data and CSV data respectively.

load.py
We are creating a class to handle MongoDB database for data loading purpose in our ETL pipeline.
Why MongoDB? It is because a schema can be inferred by our data.

transformation.py
Since transformation logic is different for different data sources, 
so we will create different class methods for each transformation.
