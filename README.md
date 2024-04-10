# Home_Sales
For this challenge, I was tasked with using SPARKSQL to determine key metrics for previous hole sales data. Using spark to create temporary vies of the data and use it to answer the folowing questions:

- What is the average price for a four-bedroom house sold for each year? 

- What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? 

- What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? 

- What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query.

I cached and validated the temporary table.

I queried for the average price of homes by it's view rating on the cached table and calculated the execution time which was 0.41 seconds. 

I then partitioned the dataset using the construction date field and read the data in parquet format. 

I re-did the same calculation using the parquet data amd took the execution time which was 1.2 seconds.

Lastly, I cleared the cache and verified it was cleared. 
