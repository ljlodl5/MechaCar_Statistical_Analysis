# MechaCar_Statistical_Analysis
RStudio and statistics support


## Linear Regression to Predict MPG

Support for Linear Regression 
![Exhibit1](https://github.com/ljlodl5/MechaCar_Statistical_Analysis/blob/main/Linear%20Estimates%20(MPG%20against%20other%20MechaCar%20Variables).png)

![Exhibit2](https://github.com/ljlodl5/MechaCar_Statistical_Analysis/blob/main/Summary%20Values%20(MPG%20Estimates).png)

1) Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Answer) Absolute non-random would be zero which is not evident from the grid. However the two numbers that are closest in addition to the intercept, is the ground_clearance and vehicle_length.

2) Is the slope of the linear model considered to be zero? Why or why not?
Answer) The slope is not zero. In order to constitute as zero slope, this would mean that mpg is not impacted by any of the factors listed. With an R2 of >.7 I anticipate some level of correlation between X and Y variables.  

3) Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Answer) With a R2 of >.7 the strength of correlation is high towards predicting mpg however despite a high R, it is important to note that additional factors/data points may draw a stronger correlation. 

## Summary Statistics on Suspension Coils


![Exhibit3](https://github.com/ljlodl5/MechaCar_Statistical_Analysis/blob/main/TotalSummarySuspensionCoil.png)



![Exhibit4](https://github.com/ljlodl5/MechaCar_Statistical_Analysis/blob/main/Lot%20SummarySuspensionCoil.png)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. 
1) Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
Answer) This variance is met by the total, however Lot 3 (@ >170.29) exceeds a variance of 100 pounds per square inch. It is importance to note while the variance exceeds the threshold when looking at the datapoints 
some of this variance is above the mean, and some below, therefore it is importance to note that while Lot 3 is more wild around the mean and a greater risk for failure ---all the points may still be well within the acceptable range (not exceeding 1600, or below 1400 psi)

   


## T-Tests on Suspension Coil

Looking at Lot 1 alone considering a P value of 1 we would assume a failure to reject the null hypothesis (i.e our sample did not provide sufficient evidence to conclude that the effect exists), but with the expansion of the other lots (Lot 2 with .6 and Lot 3 with .04) and with the total (P=.06, or 6% chance)
demonstrates a potential that the added samples provides a correlation between variables. Albeit it is important to note with a 6% opportunity of obtaining the result by chance it is slightly higher than a normal significance rate. It would be beneficial to expand the sample. 

![Exhibit5](https://github.com/ljlodl5/MechaCar_Statistical_Analysis/blob/main/ttest_all_lots.png)

![Exhibit6](https://github.com/ljlodl5/MechaCar_Statistical_Analysis/blob/main/ttest_lot1.png)

![Exhibit7](https://github.com/ljlodl5/MechaCar_Statistical_Analysis/blob/main/ttest_lot2.png)

![Exhibit8](https://github.com/ljlodl5/MechaCar_Statistical_Analysis/blob/main/ttest_lot3.png)




## Study Design: MechaCar vs Competition


1) What metric or metrics are you going to test?
Answer) When looking at whether to buy a vehicle an important quality is safety.
The data to add would include highway statistics injury/fatality count due to system failure vs. user error and would want to include make/model/year, seat count, doors (2-door/4-door) and airbags

2) What is the null hypothesis or alternative hypothesis? 
Answer) One alternate hypothesis is that airbags are not a prevention of injury/fatality.   

3) What statistical test would you use to test the hypothesis? And why?
Aswer) A t-test in order to examine the components against similar make/model (doors, size of vehicle, seat count, injury/fatality rate, airbag support) against the competition.

4) What data is needed to run the statistical test?
Answer) Examine the components against similar make/model (doors, size of vehicle, seat count, injury/fatality rate, airbag support) against the competition.
It is very possible that things I am not testing such as region where the vehicles are sold and/or average age of consumer may be more of a contributing factor than airbag distribution and car construction in preventing injury/fatalities. 

