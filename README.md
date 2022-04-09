# Amazon_Vine_Analysis

## Overview of the Analysis

BigMarket is a startup that helps business optimize their marketing efforts. One of BigMarket's clients has requested some pretty hefty analysis. The client $ellby is about to release a large catalog of products on a leading retail website. They want to know how the reviews of their products compare to the reviews of similar products sold by their competitors. They're also interested in enrolling in a program that gives out free product to select reviewers but they want to know if it's worth the cost. There are thousands of reviews and they're in words not numbers so they need to be translated for the analysis. 

### Purpose

The purpose of this analysis is to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. PySpark is used to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin and then to either use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in the dataset.


## Results

#### How many Vine reviews and non-Vine reviews were there?

- The total number of Vine reviews were 11597.

<img width="445" alt="Screen Shot 2022-04-08 at 8 35 13 PM" src="https://user-images.githubusercontent.com/95826875/162549535-4a6c1964-b006-4fea-8a7e-3fd305fe9c0c.png">

- The total number of non-Vine rewiews were 1726832.

<img width="483" alt="Screen Shot 2022-04-08 at 8 35 56 PM" src="https://user-images.githubusercontent.com/95826875/162549550-fc0825b5-44d3-458f-9bdb-01a33a4b3b1b.png">

#### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

- There were 4168 five star Vine reviews.

<img width="715" alt="Screen Shot 2022-04-08 at 8 35 40 PM" src="https://user-images.githubusercontent.com/95826875/162549558-fe2ce357-2c08-4e0c-b545-e02cd7d075b4.png">

- There were 1047970 five start non-Vine reviews.

<img width="772" alt="Screen Shot 2022-04-08 at 8 36 26 PM" src="https://user-images.githubusercontent.com/95826875/162549565-ccde5348-2a12-4a92-8f7b-8a238d060fee.png">

#### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

- 35.94 percentage of Vine reviews were five stars.

<img width="665" alt="Screen Shot 2022-04-08 at 8 36 54 PM" src="https://user-images.githubusercontent.com/95826875/162549573-d16b9947-ec64-4abf-a595-4cf5128ff660.png">

- 60.68 percentage of non-Vine reviews were five stars.

<img width="718" alt="Screen Shot 2022-04-08 at 8 37 05 PM" src="https://user-images.githubusercontent.com/95826875/162549583-c7164126-b5e8-47d2-a382-43f0abbc3696.png">


## Summary:

- Based on the results of the analysis, there is no positivity bias for reviews in the Vine program considering that 61% of the non-Vine reviews were five stars wheres as only 36% of the Vine reviews were five stars.
