# Amazon_Vine_Analysis
### 16 AWS, RDS and posgres/pgadmin

## Overview of the analysis:
Amazon has two types of reviews; 

First are those which are 'non-vine' reviews, where people simply take the time to write reviews independantly with
no paid incentive. 
 
Second are written by members of the paid Amazon Vine program. The Amazon Vine program is a 
service that allows manufacturers and publishers to receive reviews for their products. Companies (like SellBy whom we have
been working for during this module) pay a small fee to Amazon and provide products to Amazon Vine members, 
who are then required to publish a review.

We are tasked with identifying if the vine reviews are in anyway biased.

## Results of our Video Game analysis of the reviews: 

- How many total Vine reviews were there for the Video Game listing?

![Amazon_Vine_Analysis](./count_vineY.png)

- How many total non-Vine reviews were there for the Video Game listing?

![Amazon_Vine_Analysis](./count_vineN.png)

- How many Vine reviews were 5 stars that had had percent of helpful votes/total votes > .50? 

![Amazon_Vine_Analysis](./countYgt50.png)

- How many non-Vine reviews were 5 stars that had had percent of helpful votes/total votes > .50? 

![Amazon_Vine_Analysis](./countNgt50.png)

- What percentage of Vine reviews were 5 stars? 
If you take the above count of 94 and then the 48 that were 5 stars as shown below, which gives a total of 51%:

![Amazon_Vine_Analysis](./vine_Y_df5.png)

- What percentage of non-Vine reviews were 5 stars?
if you take the count of 40,471 and then the 15663 shown below that were 5 stars, which gives a total of 39%:

![Amazon_Vine_Analysis](./vine_N_df5.png)


## Vine verses non-Vine reviews Summary: 

The data shows that the vine reviews tend to have a 51% 5 star review as compared to the 39% 5 star review from
the non-vine reviews. This indicates a 12% higher 5-star reivew for vine verses non-vine reviews which is a 
significant increase. More analysis should be performed to understand these differences.

## Additional Analysis that is recommded to better understand the reviews:

1. Analysis should be done on the lower tiered reiviews as well. If there is also the same percentage difference for vine
verses non-vine video game players on the lower 1-3 star reviews then the data may not be as biased. 

2. It also, would be interesting to look at the 4 star reviews as that is also a very good rating.  Because the numbers 
above were very small when looking at the 5-star vine reviews (94 and 48), and those folks may be better or more 'educated' 
at playing video games and some of the non-vine reviewers may not be very good at video games, it may not
illustrate the entire picture very clearly.

3. Additionally, an analysis should be performed on the written reviews. By using the pySpark tools to look at the written reviews it could
reveal some more data as to why or why not the reviews are skewed to 5-stars for the vine reviewers.




