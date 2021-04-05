### Amazon Review: Analysis

## Overview of the analysis of the Vine Program

This analysis was initiated in order to better understand the value of the Amazon Vine program. This service allows manufacturers and publishers to receive reviews for their products. After paying a small fee to Amazon, companies like SellBy can provide products to Amazon Vine members who then publish a review. A specific Amazon dataset was chosen for this analysis containing reviews of grocery items. PySpark was used to perform the ETL process to extract the dataset, transform the data into dataframes, and connct to an AWS RDS instance to load the transformed data into pgAdmin. PySpark was used again to determine if there was any favorable bias toward favorable reviews from Vine members in the grocery items dataset. 

Vine_table_dataframe![image](https://user-images.githubusercontent.com/74984031/113530905-df585400-958c-11eb-8027-1fca2e2ebba3.png)


## Results 
unpaid_reviews_counts![image](https://user-images.githubusercontent.com/74984031/113530919-ee3f0680-958c-11eb-9f46-82d45defa70d.png)

paid_reviews_counts![image](https://user-images.githubusercontent.com/74984031/113530945-feef7c80-958c-11eb-9424-f82f80aeb86f.png)

- How many Vine reviews and non-Vine reviews were there?

There were 61 Vine, or paid, reviews from the dataset and 28,287 non-Vine reviews. 

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

The number of Vine reviews that were 5 stars were 20, and the number of non-Vine reviews that were 5 stars were 15,689. 

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

Five-star Vine reviews made up 32.79% of the total number of reviews. Five-star non-Vine reviews were 55.46% of the total number of reviews. 

## Summary

States whether or not there is bias, and the results support this statement. 
An additional anlysis is recommended to support the statement. 

There was a small number of Vine reviewers, or paid reviewers, out of this dataset. From this small sample, 32.79% of Vine reviewers rated products with five stars. Unpaid reviewers were more generous with their ratings, and rated products with five stars 55.46% of the time. This dataset does not demonstrate a bias on the part of Vine reviewers as the percentage of five star reviews was signficiantly less than customers leaving reviews who are not being paid for their feedback. As this is one dataset, or category, of products sold by Amazon, we cannot state with certainty that there is no bias across all products reviewed by paid reviewers. Additional product datasets would need to be analyzed in order to declare there is no bias on the part of paid Vine reviewers. 
