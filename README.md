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
## T Tests on Suspension Coils
The entire population coil test shows a small variance from the target mean of 1500 PSI.  
![t test](images/del3_test1.PNG)  
Lot 1 has a mean exact to the target PSI of 1500.  
![t test lot 1](images/del3_test_lot1.PNG)  
Lot 2 has a mean close to our target PSI of 1500. 
![t test lot 2](images/del3_test_lot2.PNG)  
Lot 3 has the greatest variance in PSI.  
![t test lot 3](images/del3_test_lot3.PNG)  
From these results, we learned that coils from lot 3 alone, have a big influence on the overall mean value of the entire population. Coils from lot 3 failed the test and should not be used during production.  
## Study Design MechaCar vs Competition
When it comes to cars and car users there are a lot of questions that come to mind, and it should. Cars are not an easy purchase, from the purpose of the vehicle to the price tag, every aspect around that car should be consider so that buyers can make an informed decision.
Nowadays the concerned for environmantally friendly products are more important to the public. For that reason, this study will focus on fuel efficiency.  
- What metric or metrics are you going to test?
    - Fuel efficiency.
- What is the null hypothesis or alternative hypothesis?
    - Are newer cars more fuel efficient?. Null hypothesis: Car age has no effect on fuel efficiency.  
- What statistical test would you use to test the hypothesis? And why?  
    - There is plenty of data regarding fuel efficiency from every car, for this reason a two-sample t test would be more appropriate.  
- What data is needed to run the statistical test?  
    - Numerical data. Eventhough I expect continuos data to be gathered, I don't want to rule out the posibility of interval data.