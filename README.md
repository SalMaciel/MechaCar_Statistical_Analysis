# MechaCar_Statistical_Analysis
## Linear Regression to Predict MPG
Using Rstudio, we will answer the following questions.
- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
    - Vehicle weight spoiler angle and and AWD have p values, greater than 0.05.
- Is the slope of the linear model considered to be zero? Why or why not?
    - The multiple R-squared value is 0.7, the linear model is not near zero.
- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
    - Overall, this linear model has a significance value lower than 0.05, which suggest that there is a strong chance that the results produced were by chance.

![Rconsole output](images/del1.PNG)
## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.
- Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
    - When we look at the total summary table, we can see that all coils meet the expectation of not exceeding the 100 PSI limit.  
![total summary](images/del2_total.PNG)  
    - However, when we inspect each lot indicidually we can see that Lots 1 and 2 meet the requirement but not Lot 3.
![lot summary](images/del2_lot.PNG)
    - Lot 3 coils should not be used during the MecaCar production as they have a variance of 170 PSI.
