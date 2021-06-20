# MechaCar_Statistical_Analysis
## Overview
AutosRUs is having production trouble with its new MechaCar and is requesting for us to create an analytical review to provide some insight. We ran the following analysis:
•	Linear Regression to Predict MPG
•	Summary Statistics on Suspension Coils PSI
•	Perform T-Tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean
•	Compare the MechaCar performance against vehicles from other manufacturers
## Linear Regression to Predict MGP
![image](https://user-images.githubusercontent.com/78935982/122677127-9a64b680-d1a6-11eb-909f-c5b43a3bde6b.png)
 
•	The most significant variables in our dataset which show a non-random effect on the MPG of the MechaCar are the Vehicle Length and the Ground Clearance. A linear regression model ran on these variables against figures for MPG, resulted in p-values of 2.6x10-12 and 5.21x10-8, respectively. The intercept was also statistically significant, indicating that there are likely other factors, not included in our dataset, that have a strong impact on the MPG.
•	The slope of the linear model can not be considered to be zero since the p-value is 5.35x10^-11 as indicated in the picture above. With that p-value, we can say the null hypothesis must be rejected and that the relationship between the variables and the MPG is subject to more than random chance.
•	Although there is still unconsidered factors, this model does predict the MPG of MechaCar with some effectiveness. With the r-squared value of 0.7149, this indicates the model is 71% effective.
## Summary Statistics of Suspension Coils
Total Summary

![image](https://user-images.githubusercontent.com/78935982/122677138-a6507880-d1a6-11eb-9c34-ad056391263c.png)
 
Lot Summary

![image](https://user-images.githubusercontent.com/78935982/122677143-abadc300-d1a6-11eb-9781-212db0081ef0.png)
 
•	While the overall variance, as shown in the Total Summary data above, is under 100 psi and meets specifications, there is a problem with lot 3. As shown in the Lot Summary stats, the variance for Lot 3 is well over the threshold, at 170.28.
## T-Tests on Suspension Coils
Summary of all Suspension Coils T-Test

![image](https://user-images.githubusercontent.com/78935982/122677161-c122ed00-d1a6-11eb-8138-f51e8cd531db.png)
 
•	The T-test for the suspension coils across all lots shows that they are not statistically different from the population mean, and the p-value is not low enough (0.0603) for us to reject the null hypothesis.
Lot 1 T-Test Summary

![image](https://user-images.githubusercontent.com/78935982/122677165-c718ce00-d1a6-11eb-9cc0-d7e8783b698c.png)
 
•	The T-test for Lot 1 shows that they are not statistically different from the population mean, and the p-value is not low enough (1) for us to reject the null hypothesis.
Lot 2 T-Test Summary

![image](https://user-images.githubusercontent.com/78935982/122677173-ce3fdc00-d1a6-11eb-8acc-891ef73776aa.png)
 
•	The T-test for Lot 2 shows that they are not statistically different from the population mean, and the p-value is not low enough (0.6072) for us to reject the null hypothesis.
Lot 3 T-Test Summary

![image](https://user-images.githubusercontent.com/78935982/122677177-d435bd00-d1a6-11eb-82c6-22a1bc627853.png)
 
•	The T-test for Lot 3 shows that they are slightly statistically different from the population mean, and the p-value is just low enough (0.0417) for us to reject the null hypothesis.
## Study Design: MechaCar vs Competition
There are many factors to take into consideration when evaluating a car to purchase. In a world where ridesharing is becoming more popular, easier and cheaper to get around in other people's vehicles, customers will be looking to buy a car that is bigger and more comfortable.
Metric to test
•	To narrow down our test, we should evaluate MechaCar's carrying capacity, in cubic inches, in comparison to various competitors' vehicles.
Null and Alternate Hypothesis
•	H0: MechaCar prototypes' average carrying capacity is similar to competitor's vehicles in the same vehicle class
•	Ha: MechaCar prototypes' average carrying capacity is statistically above or below that of competitor vehicles.
Statistical Test Used
•	The best statistical test for this would be two-sample t-tests.
What data is needed
•	We would need to gather cubic space data from the carrying compartments of all MechaCar prototypes, as well as from all major competitor vehicles.
