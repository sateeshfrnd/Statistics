# Percentiles
Percentiles are a statistical concept used to divide a dataset into hundred equal parts, each representing a percentage of the data. They provide information about how data is distributed across different segments or percentiles within the dataset.

*A Percentile is a value below which a certain percentage of observations lie.*

**Percentile rank of a number = (No. of values below that number / Total Numbers) * 100** 

Consider an example having below dataset, what is the percentile rank of 3 ? 
```
1,2,3,3, 4,5,6,7,8,9
```
Percentile rank of 3 = (2 / 10) * 100 = 20th Percentile

**What value exists at 75th Percentile**

Value = (Percentile / 100) * (n + 1) = (75 * (10 + 1)) /100 = 8.25

8th Number is '7' is 75th Percentile.

## Quartile
Quartile are the values that divides a dataset into four equal parts each representing 25% (or one-fourth) of the data. They are useful measures of spread and variability in a dataset, providing insights into the distribution of data points.

There are three quartiles commonly used in statistics:
 - **First Quartile (Q1)**: Also known as the 25th percentile, Q1 represents the value below which 25% of the data falls. It marks the boundary between the lowest 25% of the dataset and the remaining 75%.
 - **Second Quartile (Q2)**: Also known as the 50th percentile, Q2 is equivalent to the median. It represents the value below which 50% of the data falls, dividing the dataset into two equal parts.
 - **Third Quartile (Q3):** Also known as the 75th percentile, Q3 represents the value below which 75% of the data falls. It marks the boundary between the lowest 75% of the dataset and the top 25%.
 
Mathematically, quartiles can be calculated using the same procedure as percentiles, but with specific values for p (25, 50, and 75) corresponding to Q1, Q2, and Q3, respectively.

### Example
Let's consider a simple example dataset representing the scores of students in a class:

Scores: 65,72,80,85,88,90,92,95,98,100

To find the quartiles for this dataset:
- **First Quartile (Q1)**: This corresponds to the 25th percentile. We have n=10 data points, so
  - Index = (25/100) * (10+1) = 2.75
  - Since the index is not a whole number, we interpolate between the second and third data points:
    -  Q1=(72+80) / 2 =76
- **Second Quartile (Q2)**: This corresponds to the 50th percentile. which is the median. Since we have an even number of data points, the median is the average of the fifth and sixth data points:
   -  Q2=(85+88) / 2 =86.5
- **Third Quartile (Q3)**: This corresponds to the 75th percentile. Using the same method as Q1, we interpolate between the seventh and eighth data points:
  - Q3=92+(95−92)×0.5=93.5 
      
So, for this dataset, the quartiles are:
- Q1=76
- Q2=86.5
- Q3=93.5

### Five point of summary
- Minimum (Q0): The smallest value in the dataset.
- First Quartile (Q1): The value below which 25% of the data falls.
- Median (Q2): The middle value of the dataset, dividing it into two equal halves. If the dataset has an even number of observations, the median is the average of the two middle values.
- Third Quartile (Q3): The value below which 75% of the data falls.
- Maximum (Q5): The largest value in the dataset.

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/523b9af8-d284-48bc-899e-1492f3c4dc83)

**Outliers/Extream values  will lie either in Q1/Q4**

### Inter Quartile Range
The interquartile range (IQR) is a measure of statistical dispersion that quantifies the spread or variability of a dataset by focusing on the middle 50% of the data. It is calculated as the difference between the third quartile (Q3) and the first quartile (Q1), representing the range of the central half of the data.

**Inter Quartile Range = Q3 - Q1**
The IQR provides a measure of variability that is robust to outliers and skewed distributions, making it particularly useful for summarizing the spread of non-normally distributed data.

The interquartile range is often used in conjunction with box plots, where the box represents the IQR, and the whiskers extend to the minimum and maximum values within 1.5 times the IQR from the lower and upper quartiles, respectively. Outliers are plotted individually beyond the whiskers.

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/99150b66-f869-464f-b220-b20d6e449aae)

### Summary
Quartiles are commonly used in descriptive statistics and data analysis to summarize the spread and central tendency of a dataset. They are especially useful for identifying outliers, understanding the shape of the distribution, and comparing different parts of the dataset.




