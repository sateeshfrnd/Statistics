# Covariance and Correlation
Covariance and correlation are concepts commonly used in statistics to understanding relationships between variables.

## Covariance
Covariance measures the degree to which two random variables change together. It indicates the direction of the linear relationship between two variables. However, it doesn't provide insights into the strength or scale of the relationship.

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/8d26bc73-39d8-4eb3-808f-1ae80a1fcc60)

where X and Y are the variables, ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/92a8989c-2197-4f92-9cf7-dbdb8f935210) and ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/b03b5e9f-e88a-4707-a4a8-7eb8072a69ae) are individual data points, ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/1c507e4f-67d0-4dd7-9b67-895e1069c853) and ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/a77dc7da-6a95-4365-abcb-4478033e768f) are the means of X and Y, and N is the number of data points.

Covariance can take any real value, including positive, negative, or zero.
- If covariance is positive, it indicates a positive relationship between the variables.
- If covariance is negative, it indicates a negative relationship between the variables.
- If covariance is zero, it indicates no linear relationship between the variables.

**A positive covariance indicates that the two variables tend to increase or decrease together, while a negative covariance indicates that one variable tends to increase as the other decreases.**

Let's consider a simple example with two variables: 
- X representing the number of hours spent studying for an exam
- Y representing the corresponding exam scores. 

Suppose we have the following data:


X (hours)  |  Y (exam score)
--- | --- 
3|85
4|90
6|88
5|92
7|91


To compute the covariance between X and Y, we first need to calculate the means of both X and Y:

Mean of X (hours) = (3 + 4 + 6 + 5 + 7) / 5 = 5
Mean of Y (exam score) = (85 + 90 + 88 + 92 + 91) / 5 = 89.2

Now, we calculate the deviations from the means for each data point:

```
X_deviation = X - mean(X)
Y_deviation = Y - mean(Y)
```

Then, we compute the product of the deviations for each pair of data points and sum them up:

```
Sum of (X_deviation * Y_deviation)
  = (3 - 5)*(85 - 89.2) + (4 - 5)*(90 - 89.2) + (6 - 5)*(88 - 89.2) + (5 - 5)*(92 - 89.2) + (7 - 5)*(91 - 89.2)
  = (-2)*(-4.2) + (-1)*0.8 + (1)*(-1.2) + (0)*(2.8) + (2)*(1.8)
  = 8.4 - 0.8 - 1.2 + 3.6
  = 10
```

Finally, we divide the sum by the number of data points minus 1 (n - 1) to get the covariance:

```
Cov(X, Y) = Sum of (X_deviation * Y_deviation) / (n - 1)
          = 10 / (5 - 1)
          = 10 / 4
          = 2.5
```

*So, the covariance between the number of hours spent studying for an exam and the corresponding exam scores is 2.5 (positive), it suggests that students who spend more hours studying tend to achieve higher exam scores, and students who spend fewer hours studying tend to achieve lower exam scores.*

### What will be units of the covariance ?

The units of covariance are the product of the units of the two variables being measured. 

In our example, if one variable (X) represents the number of hours spent studying (measured in hours), and the other variable (Y) represents exam scores (measured in some unit like percentage or points), then the units of covariance would be the product of hours and the unit of exam scores (e.g., hours times percentage or hours times points).

For example, if the number of hours spent studying is measured in hours and exam scores are measured in points, then the units of covariance would be "hours times points." 

It's important to note that while covariance provides information about the direction of the relationship between two variables, the magnitude of the covariance is influenced by the scales of the variables, making it difficult to interpret directly. Therefore, correlation, which standardizes the relationship between two variables, is often preferred for comparisons.

```
Note: Covariance has no magnitude/dimention and depends on the units of the variables.**
```
### Summary
- One of the main disadvantages of covariance is that it is not easily interpretable or comparable across different datasets or variables with different scales.
- Covariance provides information about the direction of the relationship between two variables, it does not provide a standardized measure of the strength of the relationship.
- That's why correlation, which standardizes the relationship between two variables, is often used for comparison purposes.

## Correlation
Correlation measures the strength and direction of the linear relationship between two variables.

Formula for correlation 

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/990fb7f9-3b0e-46fe-b47a-606fed45b6cf)

where ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/6233ee38-6887-46b7-b219-0e043fb64550) and ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/d70ae2a8-3884-44fd-b238-f97ee0564e3f) are the standard deviations of X and Y, respectively.

It ranges from -1 to 1, where:
- 1 indicates a perfect positive linear relationship,
- −1 indicates a perfect negative linear relationship, and
- 0 indicates no linear relationship.

Correlation also called as Pearson correlation coefficient (often denoted as r) **always measure of the linear relationship** between two variables. It quantifies the strength and direction of the linear association between two continuous variables. 

The Pearson correlation coefficient ranges from -1 to 1, where:
- r=1: Perfect positive linear correlation.
- r=−1: Perfect negative linear correlation.
- r=0: No linear correlation.

*The Pearson correlation coefficient is commonly used in statistics and data analysis to determine the strength and direction of the relationship between variables. It assumes that the relationship between variables is linear and that the data follows a bivariate normal distribution.*

