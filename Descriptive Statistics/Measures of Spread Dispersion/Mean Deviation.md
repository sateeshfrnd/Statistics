# Mean Deviation

Mean deviation, also known as the *Mean Absolute Deviation (MAD)*, is a measure of the average absolute deviation of data points from the mean.

Mean Deviation is indeed a measure of spread or dispersion within a dataset, making it part of the broader category of measures of spread or dispersion in descriptive statistics.

The formula to calculate the mean deviation is as follows:
![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/4688f7a6-d620-4547-8856-a6251bf97ae8)


Here's how to calculate mean deviation:
1. Calculate the mean (average) of the dataset.
2. Find the absolute deviation of each data point from the mean.
3. Sum up all the absolute deviations.
4. Divide the sum of absolute deviations by the number of data points to find the mean deviation.

Let's illustrate Mean Deviation with an example:

Suppose we have the following dataset representing the scores of students in a class:

**{85, 90, 88, 92, 75, 85, 80, 78}**

**Step 1:** Calculate the Mean
```
Mean = (85 + 90 + 88 + 92 + 75 + 85 + 80 + 78)/ 8 = 673/8 = 84.125
```

**Step 2:** Find the Absolute Deviation of Each Data Point from the Mean
```
85 - 84.125 = 0.875
90 - 84.125 = 5.875
88 - 84.125 = 3.875
92 - 84.125 = 7.875
75 - 84.125 = 9.125
85 - 84.125 = 0.875
80 - 84.125 = 4.125
78 - 84.125 = 6.125
```

**Step 3:** Sum Up the Absolute Deviations
```
0.875 + 5.875 + 3.875 + 7.875 + 9.125 + 0.875 + 4.125 + 6.125 = 38.875
```

**Step 4:** Calculate the Mean Deviation
```
Mean Deviation = 38.875/8 = 4.859
```

So, the mean deviation of the student scores is approximately **4.859**. This value represents the average absolute deviation of the scores from their mean.

[Calculate Mean Deviation using Python libraries](https://github.com/sateeshfrnd/Statistics/blob/master/notebooks/Mean%20Deviation.ipynb)

## In Summary
Mean deviation is particularly useful because it gives a measure of the average distance of data points from the mean, without the need for squaring deviations as in the case of variance. It is often considered a more robust measure of dispersion, especially in the presence of outliers, as it helping analysts to better understand the distribution of the data and make informed decisions based on its characteristics.



