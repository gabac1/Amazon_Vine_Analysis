# Amazon Vine Analysis
## Overview of the analysis of the Vine program:
The purpose of this analysis is to determine whether reviewers' enrolment in the amazon vine program create a bias in the reviews they write. From the amazon reviews data of kitchen products, the subset in which each review has more than 20 total votes is drawn and used in this analysis, to ensure the quality of the study.
The data is hosted on AWS cloud and the ETL process is done on Google Colab.
## Results:
In the selected sample, there are in total 1160 reviews written by amazon vine members and 92308 reviews written by non-vine users. The number of 5-star reviews in the vine member group is 489 (42.16% of the vine reviews), whereas the number of 5-star reviews in the non-vine group is 43247 (46.85% of the non-vine reviews). 

Table 1: reviews from vine program 
| Star Rating | Number of Reviewers | Proportion in Total |
| :------------- |:-------------| :-----|
| 1 | 42 | 0.036207 |
| 2 | 68 | 0.058621 |
| 3 | 214 | 0.184483 |
| 4 | 347 | 0.299138 |
| 5 | 489 | 0.421552 |

Table 2: reviews from non-vine consumers
| Star Rating | Number of Reviewers | Proportion in Total |
| :------------- |:-------------| :-----|
| 1 | 21201 | 0.229677 |
| 2 | 6855 | 0.074262 |
| 3 | 8133 | 0.088107 |
| 4 | 12872 | 0.139446 |
| 5 | 43247 | 0.468508 |

However, although the number of 5 star votes is not higher in the vine group, the distributions of star ratings of the two groups are very different. The percentages of 4 and 3-star ratings in the non-vine group are lower and the percentage of 1-star ratings is much higher than in the vine group, as can be observed from the following figures.
![Figure 1](https://github.com/gabac1/Amazon_Vine_Analysis/blob/main/resources/fig1.svg)
![Figure 2](https://github.com/gabac1/Amazon_Vine_Analysis/blob/main/resources/fig2.svg)
## Summary:
In sum, although the percentage of 5-star ratings in the vine reviewers group is not higher than in the non-vine group, the possibility of a bias cannot be ruled out, since the rating distributions of the two groups differ in general.
