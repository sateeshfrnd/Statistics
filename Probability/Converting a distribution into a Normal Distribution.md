# Converting a distribution into a Normal Distribution

There are several techniques used to convert the distribution of data to approximate a normal distribution. If you are modelling statistical ML model then data should follow Normal Distribution.

Some common techniques include:

# Transformations
Converting a distribution into a normal distribution typically involves applying transformations or adjustments to the data to make it resemble a normal distribution more closely. Some common techniques to achieve this include:

### Logarithmic Transformation
   - If the data is positively skewed, taking the logarithm of the data can reduce the skewness and make the data more normally distributed.
   - This can be particularly useful for data that follows an exponential distribution.
### Square root transformation
   - Similar to the logarithm transformation, taking the square root of each data point
   - Useful for stabilizing variance and making data more symmetric.
   - This can be particularly useful for count data or data that follows a Poisson distribution.

### Box-Cox transformation
- The Box-Cox transformation is a power transformations that can handle different types of transformations, including logarithmic and square root transformations.
- It selects the best transformation parameter to make the data most closely resemble a normal distribution.

### Reciprocal Transformation 
- the Reciprocal Transformation involves taking the reciprocal (1 divided by the original value) of each data point.
- It's useful when dealing with highly skewed data with a long right tail, as it can help make the distribution more symmetric.
- Logarithmic/SquareRoot Transformation do not adequately address the skewness in the data, the reciprocal transformation can be considered as an alternative.
  
### Johnson transformation
- The Johnson transformation is often used in situations where traditional methods, such as log transformation or Box-Cox transformation, are not effective in normalizing the data. 
- It involves applying a four-parameter transformation formula to the data to achieve symmetry and constant variance.
- This transformation helps improve the validity of statistical analyses that rely on the assumption of normality.
- It may also introduce new challenges, such as handling zero values (since the reciprocal of zero is undefined) or amplifying variability in the data. 

**Which Transformation When ?**
Distribution | Transformation 
--- | --- 
Right Skew Data | Logarithmic/SquareRoot Transformation 
Left Skew Data | Reciprocal Transformation 
Positively Skew Data | Box-Cox  Transformation 
Nagitive Skew Data | Johnson transformation Transformation 
Non zero Data | Reciprocal Transformation 

It's important to note that these transformations can be data-dependent and may require some trial-and-error to find the best transformation for a given dataset. Additionally, it's important to understand the underlying data-generating process and whether a normal distribution is appropriate for the data before transforming the data.

## Scaling
### Standardization (Z-score)
- Standardizing the data by subtracting the mean and dividing by the standard deviation transforms the data into a standard normal distribution with a mean of 0 and a standard deviation of 1.
- Useful for comparing variables with different units and for algorithms that rely on distance measures.

### Normalization (Min-Max Scaling)
- Min-max scaling, also known as normalization, is a data preprocessing technique used to rescale numerical features to a specific range, typically between 0 and 1.
- Useful for algorithms that require input features to be within a specific range.

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/63db40d1-c39c-41e3-a01b-b1ad03f3d381)

where
- x: The original value of the feature.
- min: The minimum value of the feature in the dataset.
- max: The maximum value of the feature in the dataset.
- x scaled : The scaled value of x within the range [0, 1].

**Note: If outlier then go with Standardization otherwise Normalization.**
  
## In Summary
These techniques are commonly used in data preprocessing, exploratory data analysis, and statistical modeling to prepare data for analysis, address issues such as unequal spread or variability of residuals (the differences between observed and predicted values) and non-normality, and improve the performance of statistical models. Choosing the appropriate technique depends on the characteristics of the data and the goals of the analysis.
