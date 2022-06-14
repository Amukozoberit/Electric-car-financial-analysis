# Electric-car-financial-analysis
Problem statement
We have been tasked to understand electric car usage. We will work as a Data Scientist for the Autolib electric car-sharing service company to investigate a claim about the blue cars from the provided Autolib dataset.
 
In an effort to do this, we need to identify some areas and periods of interest via sampling stating the reason to the choice of method, then perform hypothesis testing with regards to the claim that we will have made. An example of claim to test would be "Is the number of Bluecars taken in area X different than in area Y? Is it greater in area X than in area Z? Etc”. The selected periods of interest be either weekdays or weekends but not a mix of both. You can also consider postal codes 75015 vs 75017 to some of the areas of interest.
 
 
 
We are investigating the blue cars with regard to  daytype and the area.
 
 
## Null Hypothesis
**There is no diffrence between the blue cars taken in area 92000 and 94700 during the weekend**
 
##  Alternate Hypothesis
**There is a difference between the blue cars taken in area 9200 and 94700 during the weekend**
 
 
 
## Importance:
Weekends according to our data has more sum therefore we take the weekend,we investigate the cars taken because our aim is to increase the blue cars taken.
 
 
 
## Data Description
We need data with the following Postal code dayOfWeek,BlueCars_returned_sum,'BlueCars_taken_sum,day_type
 
In the descriptive statistics we have cleaned the data,removed unused columns,visualized columns.The data is provided by the autolib company.
 
 
 
## Hypothesis testing procedure
#### 1. Define problem statement
#### 2. Defining Hypotheses
Create and u nderstand a scientific question we are looking for.
Null and alternative hypothesis defined
 
#### 3. Decide on the significance level==0.05%
#### 4.Check the assumptions
To use a test it has to pass certain conditions.In our test we perfomed the shapiro test provided by scipy to find out if the data is normally distributed.then used aggregation tests to check for the count of the samples which was >30 and the data was not normaly distributed
 
#### 5.Choose test
 
5.1. When population std is known we use z-test
data should be normally distributed and sample >30
 
5.2. t-test
When population std is not known we use t-test
data should be normally distributed and sample <30
 
5.3. Mann-Whitney U test
When population std is not known we use t-test
data **should not be normally** distributed and sample <30
 
Conclusion-Mann-Whitney U test also we used 2 tail test because our data was testing on equality and not greatness.
 
 
 
 
 
 
 
 
 
 
## 6.0. Calculate the test
We calculated the test and got
MannwhitneyuResult(statistic=4570.0, pvalue=0.0)
 
 
## Hypothesis test results
 
 
In our case p value is 0.0 which is less than significant 0.05 therefore There is no enough evidence to prove H₀ is not valid,therefore we reject the null hypothesis and accept the alternative hypothesis.
 
## Summary and Conclusions
In the project we collected data performed data exploration and cleaning then performed a hypothesis test to it.The test involved creating a null and alternative hypothesis then calculating the p value to compare with the significant value.If the p-value is smaller than the alpha (the significance level), in other words, there is enough evidence to prove H₀ is not valid; you can reject H₀. Otherwise, you fail to reject H₀.


<a href="https://docs.google.com/document/d/1-C_RGBTcK4uoNXEdb1LyXa2Cwzz5_yQCCtmYH-UT39Y/edit" target="_blank">Find the full document here</a>
