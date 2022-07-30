# Amazon_Vine_Analysis

## Purpose

The purpose of this analysis is to choose from 50 different datasets for AMAZON VINE and utilize PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS(Relational Database Service) and load the transformed data in pgAdmin.  Using PySpark to determine if there was any bias towards providing favorable reviews in the selected dataset.

## Results

## Deliverable 1:  Perform ETL on Amazon Product Reviews

For this Deliverable, I created an AWS RDS with the tables created/framed in pgAdmin, awaiting data to be written in to their respective tables.  I transformed the data frame into four seperate data from that match the schema of pgAdmin(AWS Server: AWS_FRIDAY, Database: RW1, Schema: public)   

![image](https://user-images.githubusercontent.com/8845050/181936030-9710e4d8-eeec-45be-8719-d63f8b7b7ac9.png)

### Customer Dataframe
![image](https://user-images.githubusercontent.com/8845050/181936137-f800c107-bc5a-43fc-a879-1a2ce790323e.png)

### Products DataFrame
![image](https://user-images.githubusercontent.com/8845050/181936201-4aa9a8af-98c8-4006-a10f-4c1126ed91c0.png)

### Review_ID DataFrame
![image](https://user-images.githubusercontent.com/8845050/181936217-31e71f56-8b0e-4db7-acfb-b6fe21c755ae.png)

### Vine DataFrame
![image](https://user-images.githubusercontent.com/8845050/181936277-63667428-2dd1-4649-9892-4a5222ecf070.png)

### From PgAdmin----------------------------------------------------------------------

### Customers Table:
![pg_customers_table](https://user-images.githubusercontent.com/8845050/181962011-c44d85a0-686a-4a1e-9e93-5ed441bbf9d8.PNG)

### Products Table:

![pg_product_table](https://user-images.githubusercontent.com/8845050/181962260-e60f6e8b-9ad4-40a6-a715-992947e4304e.PNG)

### Review ID Table:

![pg_review_id](https://user-images.githubusercontent.com/8845050/181962918-66d1fba9-cc5d-45f2-83ae-36b201be87f2.PNG)

### Vine Table:

![pg_vine_table](https://user-images.githubusercontent.com/8845050/181963776-b96eebc7-e913-4564-8ca3-769cb20a03f6.PNG)

### Non-Vine(N) Table:

![image](https://user-images.githubusercontent.com/8845050/181995932-6b2c99f5-53e2-410b-b2ef-f8d1fba1b1f4.png)

### Vine(Y) Table:

![image](https://user-images.githubusercontent.com/8845050/181995916-12e81afb-1415-4b3c-8834-665f8fb5f0d1.png)

# Deliverable 2: 

Using Pyspark (Google Collaboratory), I calculated whether or not there was any bias towards reviews that were written as part of the Vine Program and if having a PAID VINE REVIEW made any difference in the percentage of 5-star reviews.

* For Deliverable 2, there were:
  * Total Vine Reviews: 47
  * Total Non-Vine Reviews: 8362
  * Total Vine 5-star reviews: 15
  * Total Non-Vine 5-star reviews: 4332
  * Percentage of Vine 5-star reviews = (5 star Vine / Total Vine) = 31.92%
  * Percentage of Non-Vine 5-star reviews = (5 star Non-Vine / Total Non-Vine) = 51.81%

# Summary

According to the data, despite the Vine percentage being around 32", there is not correlated bias with "Paid reviews equating to higher ratings(stars)". because NON-PAID has a 5-star rating of roughly 52%, which is higher than the 5-star/paid ratio.  The only further analysis I would like to see is that there is more data(counts) in the TOTAL PAID REVIEWS.  A sample of just 47 may not give a clear picture, but conceding to a T Test showing that the sample is a good representation of the population, then I would agree that there is NO BIAS within the data on given PAID-NON-PAID reviews.

Visualizations of a tsacked bar chart or bubble chart would show the important factors that we may not be looking at in this simple analysis.   Expanding the analysis fields to capture more data, or using a larger sample size would shed more light and give further confidence to the results.

# Resources

 * Google Colaboratory
 * pgAdmin 4
 * PySpark version 3.3.0








