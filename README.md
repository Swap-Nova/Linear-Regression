- Linear Regression analysis is used to predict the value of a variable based on the value of another variable.
- The variable you want to predict is called the dependent variable. The variable you are using to predict the other variable's value is called the independent variable.

## Main idea behind using this classification model:
The goal here is to predict the mouse size using mouse weight. 
1. Drawing a line through the data
2. We measure the distance from line to data, then square each distance and add them up. Distance from line to data point is called a ```Residual```
3. We rotate the line, and with this new line we measure the residuals, square them, and sum the squares present
4. Rotate the line a bit more, and sum up the square residual. We have done this for some time. After a bunch of rotations, we can plot the sum of squared residuals and corresponding rotation.
<center><img width="400px" alt="Screenshot 2023-12-12 at 8 25 50 AM" src="https://github.com/Swap-Nova/Linear-Regression-/assets/92979885/62c91bae-e78d-40b6-93a2-a725d0897937"></center>

- We find the rotation that has the least sum of squares. So this will be able to fit to data. The method for fitting a line is called ```Least Squares```

## Linear Regression in R:
- R will plot out the data frame where we will set up our linear regression. Here lm stands for linear model and we pass the formula where we pass the mouse data.
- Here: y-vaules= y-intercept + slope+x-values
- The LM function calculates the least square estimate for y-intercept and slope. Then we generate a summary of the regression. 
