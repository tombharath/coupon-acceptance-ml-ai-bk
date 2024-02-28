# coupon-acceptance
This is a practical use-case application for Data Analysis skills.  

## Will a Customer Accept the Coupon?

**Context**

Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving. Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?


**Data Cleaning**

- 74 duplicates are removed from the data set
- The Car column has 99% data which is null. The field is dropped assuming the driver can have any vehicle.
- The columns Bar, CoffeeHouse, CarryAway, RestaurantLessThan20, Restaurant20To50 are having NaN value less than 2 %
- Imputing those columns with NaN with the most occurrence of the value for that column

**Code**
- Refer to prompt.ipynb for the jupyter notebook for the python code.
- The code uses Plotly express libraries. As GitHub doesn't display plotly chart correctly. The renderer is used to show it as a picture.
- You can change the fig.show("png") to fig.show() in the jupyter notebook python code to have the hover functionality while running it.
 
 ## Observations Summary

The acceptance rate of the coupon is 56.76 %

 ![image](https://github.com/tombharath/coupon-acceptance-ml-ai-bk/assets/37302704/83e6a4d9-9c3b-4472-b15c-5750486b5257)

## Bar Coupons Analysis  Observations

1. The Bar Coupon has a 41 % Acceptance Rate
   
![image](https://github.com/tombharath/coupon-acceptance-ml-ai-bk/assets/37302704/8db21066-16b4-469e-ad50-252b2a7a148c)

2. The acceptance rate is higher for those who went to a bar 3 or fewer times a month when compared with those who went more than 3 times
   
![image](https://github.com/tombharath/coupon-acceptance-ml-ai-bk/assets/37302704/a3668c9b-416c-4760-a10d-42e8875b8d0a)

3. There is no difference in the acceptance rate for those who are over the age of 25 based on the frequency of visits and the same for those who are under 25 as well.
   
 ![image](https://github.com/tombharath/coupon-acceptance-ml-ai-bk/assets/37302704/9ca09c8d-29c3-4dd4-9443-412c79850dbe)

4. The acceptance rate for drivers who had passengers who were not a kid and had occupations other than farming, fishing, or forestry is similar (22%) irrespective of whether they go more than once or less than once a month.

![image](https://github.com/tombharath/coupon-acceptance-ml-ai-bk/assets/37302704/b2227998-92a4-4ffc-86ce-f248c7b4bb91)

6. The acceptance rates for drivers who go to bars more than once a month and are under the age of 30 are slightly higher acceptance rate(28%) compared to drivers who go to bars more than once a month, had passengers who were not kids, and are not widowed(22%) and drivers go to cheap restaurants more than 4 times a month and income is less than 50K.
   
![image](https://github.com/tombharath/coupon-acceptance-ml-ai-bk/assets/37302704/85249f2a-58d4-4a70-9431-0421e8d8d472)

## Coffee House Coupon Observations

1. The Coffee House Coupon has a 50 % Acceptance Rate

![image](https://github.com/tombharath/coupon-acceptance-ml-ai-bk/assets/37302704/066bd001-c571-4618-9dea-a59d489c55d3)

2. Surprisingly 80 % of drivers tend to accept the coupon even if the venue is in the opposite direction

![image](https://github.com/tombharath/coupon-acceptance-ml-ai-bk/assets/37302704/d91226a7-ced5-47fb-8984-5f1cf7f9f3ec)

3. The Acceptance rate is higher for No Urgent Destination and lower for the people who are going home

![image](https://github.com/tombharath/coupon-acceptance-ml-ai-bk/assets/37302704/a62997e6-7d34-4df3-9f8f-96b5f64a8ce0)

4. More people go to the venue within 5 minutes of travel duration

5. The Driver with Kids or Alone has a higher acceptance percentage and prefers to go there during Sunny weather.

![image](https://github.com/tombharath/coupon-acceptance-ml-ai-bk/assets/37302704/eaba1d3f-3b0b-4ec4-a796-cf619d111d0d)

6. The Acceptance Rate is higher for the driver in the below occupation irrespective of the passenger in the car. 
- Healthcare Support
- Healthcare Practitioners & Technical
- Management
- Arts Design Entertainment Sports & Media
- Computer & Mathematical
- Life Physical Social Science
- Personal Care & Service
- Community & Social Services
- Sales & Related

![image](https://github.com/tombharath/coupon-acceptance-ml-ai-bk/assets/37302704/2516db17-717a-4071-bdbd-a7b1edeae6c2)
