# Variance
Variance is a measure of the dispersion or spread of a dataset around its mean. It quantifies how much the data points in a dataset differ from the mean on average. 

**In simpler terms,The average of the spread difference between each data point and the Mean**

Mathematically, variance ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/a5d85917-db15-4789-abd6-0e4318d0ce57) is calculated as the average of the squared differences between each data point and the mean of the dataset. For a dataset with n data points and mean μ, the variance is given by:

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/77512caa-d86e-42ce-90fb-a11709a81827)


Where
- ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/c51641cf-c0cd-4dd6-8150-2e166661c2e4) represents each individual data point in the dataset.
- μ is the mean of the dataset.
- ∑ denotes the summation over all data points.

## Why the difference in the divisor for calculating population variance (N) and sample variance (n−1) arises ?

The difference in the divisor for calculating population variance (N) and sample variance (n−1) arises from the concept of **degrees of freedom** and the **desire to obtain unbiased estimates of variance**.

### unbiased estimate of the variance
*An unbiased estimate of the population variance means that, on average, the estimate obtained from the sample accurately reflects the true variability present in the entire population.*

Let's consider a simple example, you want to estimate the average height of all students in a school. Instead of measuring every student (which would be impractical), you take a random sample of students and calculate their average height. If you repeat this process many times, the average of all those sample averages will be very close to the true average height of all students in the school. This unbiasedness ensures that your sample provides a reliable estimate of the population parameter.

Similarly, when estimating the population variance using a sample, an unbiased estimate ensures that, on average, the variance calculated from the sample accurately reflects the true variability present in the entire population. This is important for making accurate statistical inferences and drawing conclusions based on sample data.

### degree of freedom 
Degrees of freedom (df) represent the number of values in a sample that are free to vary after certain restrictions or conditions are imposed. In simpler terms, it is the number of observations in the sample that can vary independently.

### Population Variance (![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/034ee8e8-776d-4339-84ad-f84a01827cb6))
When calculating the population variance, we divide by N, where N is the total number of observations in the population. 

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/77512caa-d86e-42ce-90fb-a11709a81827)

This is because the population variance aims to estimate the true variability within the entire population. Dividing by N provides an **unbiased estimate of the population variance**.

### Sample Variance (![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/1587ddcd-b6c0-4eb0-84b8-849d6c4ddd58))

When dealing with a sample of data rather than the entire population, we typically use the sample variance, which estimates the variability within the sample. In this case, we divide by n−1 instead of n to account for **the loss of one degree of freedom**. 

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/21ac3a57-826d-44a1-9547-46a22025f1d9)


The adjustment of dividing by n−1 instead of N in sample variance calculations is known as Bessel's correction, and it ensures that the sample variance provides an unbiased estimate of the population variance. This correction accounts for the fact that using the sample mean instead of the population mean tends to underestimate the true variance, particularly in smaller samples.


## Summary
Variance is widely used in statistics and data analysis to understand the variability within a dataset. However, because it is in squared units. This makes variance less intuitive for interpretation because it is not on the same scale as the original data. 

Therefore, the square root of the variance, known as the standard deviation. *By taking the square root, the standard deviation is in the same units as the original data, making it more interpretable.* It represents the average distance of data points from the mean in the same units as the data.

While variance is mathematically useful and often used in statistical calculations, standard deviation is preferred for interpretation and communication of results because of its direct relationship with the original data's units. It provides a more meaningful measure of the spread of data and is easier to understand for non-statisticians.
