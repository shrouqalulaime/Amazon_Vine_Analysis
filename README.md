# Amazon_Vine_Analysis

## Overview of the analysis
 The project aims to determine if there is any bias toward favorable reviews from Vine members in Amazon reviews data of health personal care products. The data are stored in Amazon S3. The following tasks are done to complete the data preparation and analysis:

 1. Use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin.
 2. Use PySpark, to determine if there is any bias toward favorable reviews from Vine members by calculating the percentage of Vine and non-Vine reviews that were five stars. 

## Results
The analysis results of Vine program data indicated that:

- The total number of Vine and non-Vine reviews are 32,026 and 5,299,189, respectively.
- The total number of Vine reviews that were five stars is 13,127.
- The total number of non-Vine reviews that were five stars is 3,344,959.
- The percentage of Vine reviews was five stars is 41%, whereas the percentage of 5 stars for non-Vine reviews is 63%.

<img width="1041" alt="Screenshot 2023-01-07 at 9 07 20 PM" src="https://user-images.githubusercontent.com/48078471/211181445-20066554-1985-45f6-b6cb-fcf5f6a436bf.png">

## Summary

The analysis results indicate a bias in the Vine program data, as most data is for non-Vine users. In addition, the sample size of Vine reviews is considerably smaller than non-Vine users. 
Additional analysis might be done to perform random undersampling of the non-Vine users to match the sample size of Vine users and repeat the analysis of calculating the percentage of 5 stars reviews for each type.