# Practical_Application_Assignment_5p1
Practical assignment of Module 5 of UC Berkeley Professional Certificate on ML and AI

Link:
https://github.com/tolispapathan/Practical_Application_Assignment_5p1

Overview:
- In this assignment, the goal is to analyze data related to the acceptance of coupons delivered to drivers in the vicinity of a number of stores such as restaurants and coffee houses. The target is to use what was taught about data visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not. This data is taken from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk: The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver.

Included files:
1. README.md (this file)
2. CSV data file: coupons.csv
3. Python notebook: Practical_Application_Assignment_5p1_ipynb.ipynb

Key observations:
A. Based on the problems that had to be solved:
- Data cleaning:
  1. Since the percentage of null values for column "car" was very high (>99%), removed this column from the dataframe
  2. For the columns that had a relatively small percentage of null values (<2%), it seemed reasonable to set all the null (nan) values to 'never', which was an existing category in all those columns.
- The proportion of the total observations that chose to accept the coupon is 56.84 %.
- There is significant sensitivity to whether a coupon is accepted only for cheap restaurants (< $20) and 'Carry out & Take away' stores.
- The coupon is clearly accepted at higher rate when the temperature is high (at 80 degrees).

B. Based on the investigation of the bar coupons:
- The proportion of bar coupons that were accepted is 41.00 %.
- Based on the analysis of the data, I would hypothesize that drivers who accepted the bar coupons are likely to be over the age of 25, go to a bar more than once a month, and do not have kid passengers in the car.

C. Based on the independent investigation of the Coffee house coupons:
- From analyzing the data for the Coffee House coupons, the following main observations can be made:
  1. Drivers are more likely to accept the coupon when they have friend passengers and less likely to accept when they are alone.
  2. Drivers are more likely to accept the coupon at 10 am and 2 pm than earlier or later times in the day.
  3. Only drivers of age below 21 years show are significantly more likely to accept the coupon than any other age.
  4. Drivers are more likely to accept the coupon when it has longer expiration time (1 day vs. 2 hours).
  5. Drivers are more likely to accept the coupon when their income is less than 62.5K or higher than 100K.
