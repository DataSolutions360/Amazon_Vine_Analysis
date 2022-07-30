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

### From PgAdmin-------------------------------------------------------------------------------------------------

### Customers Table:
![pg_customers_table](https://user-images.githubusercontent.com/8845050/181962011-c44d85a0-686a-4a1e-9e93-5ed441bbf9d8.PNG)

### Products Table:

![pg_product_table](https://user-images.githubusercontent.com/8845050/181962260-e60f6e8b-9ad4-40a6-a715-992947e4304e.PNG)

### Review ID Table:

![pg_review_id](https://user-images.githubusercontent.com/8845050/181962918-66d1fba9-cc5d-45f2-83ae-36b201be87f2.PNG)

### Vine Table:

![pg_vine_table](https://user-images.githubusercontent.com/8845050/181963776-b96eebc7-e913-4564-8ca3-769cb20a03f6.PNG)


# Deliverable 2:  







