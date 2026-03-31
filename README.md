# 6211_Forecasting_lesson
This is the codebase used during the lecture on times series forecasting in the DSBA 6211 Class

*Round 2: Discussion*
Which Coefficients are statistically significant? Trend, Seasonal dummies, or both?

In a pure linear model, the Trend P-value is 0 or very close to 0 so it is significant since P<0.05

![alt text](images\output_3.png)

In a seasonality model, the Seasonal P-value for February is greater than 0.05 so it is not significant, however the rest of the months have a P-Value less than 0.05 giving them statistical significance in this model.

![alt text](images\output_2.png)

In a polynomial trend + seasonality model, the np.square(trend) has a P-Value of 0.739 which tells us it is not significant. np.square(trend) is the trend variable squared which means it represents quadratic time trend / curvature or acceleration of the model. 

![alt text](images\output.png)

How does the trend-only model compare to the seasonality-only model in validation RMSE?

Why might adding both trend AND seasonality improve accuracy?

What can you learn from the monthly coefficients?