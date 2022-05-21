# MechaCar_Statistical_Analysis
## Overview
The goal of the project is to analyze metrics that can affect the manufacturing a new car prototype and compare vehicle performance across different manufacturer lots. These metrics include vehicle length, weight, spoiler angle, ground clearance, AWD capabilities, MPG, and PSI.

## Linear Regression to Predict MPG

### Linear Regression
![Screenshot (77)](https://user-images.githubusercontent.com/94252681/169633838-fd652db5-e383-4425-b630-9600b2c7d540.png)

##### 3 Key Takeaways:

Variance of a non-random variable is usually 0. Given this fact, the intercept, vehicle_length, and ground_clearance coeeficients can be said to provide a non-random amount of variance to the mpg values.
At a significance level of 0.05, we are able to reject the null hypothesis because of the extremely small p-value. The null hypothesis of a linear regression states that the slope (β1) is equal to 0. However, if we reject the null hypthesis, we're stating that alternative (β1 ≠ 0) is true. Thus, proving that the slope is not 0.
Multiple R-squared increases as more variables are passed through the regression. However, adjusted R-squared controls against this increase, and adds penalties for the number of predictors in the model, thus making it a more accurate predictor of how effective the linear model is. An adjusted R-square of 0.6825 concludes that this linear model predicts the mpg of MechaCar prototypes relatively well.

## Summary Statistics on Suspension Coils
![Screenshot (84)](https://user-images.githubusercontent.com/94252681/169633848-ba5b4dcb-e455-45e1-bc30-2f9ba54e6473.png)
![Screenshot (85)](https://user-images.githubusercontent.com/94252681/169633850-6be690c3-6d79-468d-b6b0-e4832d107c33.png)

The overall variance for the entire dataset indicates that the current manufacturing data meets the 100 pounds per square inch variance limitation. However, when separated into three lots, the third lot demonstrates a much higher variance. Because the lots are chosen randomly, there is a possiblity that a third of the lot does not meet the necessary suspension coils requirement.

### T-Test on Suspension Coils

![Screenshot (78)](https://user-images.githubusercontent.com/94252681/169633799-45cece9b-58e3-4180-af1e-c4dc81b9d527.png)

### T-Test on Entire Lot

At a significance level of 0.05, we fail to reject the null hypothesis since the p-value equals 0.06. Therefore, we cannot reject the fact that the sample mean may be equivalent to the true population mean. Another feature to note is the narrow confidence interval. Although a narrower confidence interval implies that there is a smaller chance of obtaining an observation within that interval, it provides greater accuracy than a wider interval.
### T-Test on Three Smaller Lots
![Screenshot (87)](https://user-images.githubusercontent.com/94252681/169633912-02301d38-180c-4c30-a875-7770e86cb603.png)

#### Lot 1 
At a significance level of 0.05, we fail to reject the null hypothesis since the p-value equals 1. An interesting correlation between p-value and confidence intervals is that as the p-values get larger, the confidence interval becomes smaller, implying more precision in predicting the true population mean.

#### Lot 2
At a significance level of 0.05, we fail to reject the null hypthesis again since the p-value equals 0.6072. The second lot also has a relatively small confidence interval.

#### Lot 3
At a significance level of 0.05, we can reject the null hypothesis since the p-value equals 0.04168. The mean of this sample is also significantly smaller in comparison to the previous two lots. More importantly, unlike the previous two lots, the confidence interval for the third lot does not include the predicted population mean.

## Study Design: MechaCar vs. Competition
Another statistical study that can be performed to determine MechaCar's standing against its competition is a linear regression on city and highway fuel efficiency. Gasoline is expensive nowadays, and it is an important feature that many consumers look at when purchasing a new car. The metrics that can be included in this analysis are:

City and highway fuel efficiency: dependent variable
Horse power: independent variable
Vehicle weight: independent variable
AWD capabilities: independent variable
MPG: independent variable In addition to the MPG, AWD, and vehicle weight data that we already have, we would have to collect fuel efficiency and horse power data for the sample data set at hand.
