# Amazon_Vine_Analysis
# Background

This project aim is to analyze a dataset from the Amazon Vine program (https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt) using PySpark for ETL performing and dataset extraction, followed by AWS RDS instance connection and loading the transformed data into pgAdmin. Additionally, it is to make sure whether this dtat has any bias toward favorable reviews from Vine members using PySpark, Panadas, or SQL.

# Results
# Deliverable-1: Perform ETL on Amazon Product Reviews

## The customers_table DataFrame
![Customer Table](https://user-images.githubusercontent.com/100442163/175123649-b9c23149-bf4a-4e3c-8191-155d5f8ca5be.png)

## The products_table DataFrame
![Product_table](https://user-images.githubusercontent.com/100442163/175123917-35762b55-201b-4073-9af0-3d19e65e4e5c.png)

## The review_id_table DataFrame
![review_id_table](https://user-images.githubusercontent.com/100442163/175124158-0bee5aac-4bfb-4ed0-b405-5ab5ecf04a0a.png)

## The vine_table DataFrame
![vine_table](https://user-images.githubusercontent.com/100442163/175124399-1ddab318-0114-4e2e-a7e0-f56e9037bc18.png)

# Deliverable-2:
## How many Vine reviews and non-Vine reviews were there?
Vine members made up only 0.23% (94) of the reviews whereas the remaining 99.7% were Non-Vine members (40,471).
![Q-1](https://user-images.githubusercontent.com/100442163/175320005-737082fa-0573-4e1e-a4b1-7ed048247756.png)
![Q1b](https://user-images.githubusercontent.com/100442163/175323293-c97fb2aa-cd7c-4e8d-917e-39adee8a0dd6.png)
![Q1c](https://user-images.githubusercontent.com/100442163/175323702-bc8a842e-d794-4cbf-a926-bb786a08f04a.png)

## How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
1. Vine members gave 48 out of 94 reviews a 5 star rating.
2. Non-Vine members gave 15,663 out of 40,471 reviews a 5 star rating.

## What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
1. 51.06% of the reviews for Vine members were rated 5 stars.
1. 38.7% of the reviews for Non-Vine members were rated 5 stars.


# Summary
Although ~50% vine members gave 5-star rating which is significantly higher than non-vine member's 5-start rating percentage (i.e., 38.7%), it will not significantly impact on the over-all rating since total vine members participation was very low (i.e., 0.23% of the total voters). 
