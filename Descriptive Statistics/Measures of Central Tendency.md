# Measures of Central Tendency
Measures of central tendency are statistical measures that represent the central or typical value of a dataset. They provide insights into where the data cluster around and are used to summarize the central position of the distribution. 

The three most common measures of central tendency are:
1. Mean
2. Median
3. Mode


## Mean (Arithmatic Mid value of data)
   - The mean, also known as the population mean or μ (mu), represents the average value of a variable in an entire population.
   - It is calculated by summing all the values in the dataset/population and dividing by the number of values.
   - It is sensitive to extreme values (outliers) and can be affected by skewed distributions.
   - Formula for the population mean is:

     ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/bed26098-53a5-4e48-8ccc-b540ba6080c8)

     where ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/0223cf8b-0520-44f9-92f1-1b64a5ac229e) represents each individual value in the population, and *N* represents the total number of values in the population.

### Sample Mean
- The sample mean represents the average value of a variable in a sample of data drawn from a larger population.
- It is calculated in a similar manner to the population mean, but it uses the data from the sample rather than the entire population.
- Formula for the sample mean is

  ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/a103d8af-daa9-4835-9c3a-cba11b34a932)

   where ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/0223cf8b-0520-44f9-92f1-1b64a5ac229e) represents each individual value in the sample, and *n* represents the total number of values in the sample.

### Population Mean VS Sample Mean
- The population mean describes the average value of an entire population, whereas the sample mean describes the average value of a sample drawn from that population.
- The population mean is a fixed value that represents the true average of the population, while the sample mean can vary from one sample to another.
- When calculating the sample mean, we typically use the symbol ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/0223cf8b-0520-44f9-92f1-1b64a5ac229e)  to distinguish it from the population mean *μ*.

In summary, the mean and sample mean both provide measures of central tendency, but they apply to different contexts: the entire population and a sample drawn from that population, respectively.

### Mean is influenced by the outlier
Consider the following dataset representing the ages of ten individuals:
{18,20,21,22,23,24,25,26,27,100}

Without the outlier (100), the mean age is: (18+20+21+22+23+24+25+26+27) / 9 = 23.44
However, when we include the outlier (100), the mean age becomes: (18+20+21+22+23+24+25+26+27+100) / 10 = 34.6

As you can see, the outlier (100) significantly increases the mean age from 23.44 to 34.6. This illustrates how outliers can skew the mean towards extreme values. In this case, the mean no longer accurately reflects the central tendency of the data, as it is *heavily influenced by the outlier*.

Outliers can distort the mean because the mean is calculated by summing up all values and dividing by the total number of values. Outliers, being much larger or smaller than the other values, disproportionately affect the sum, leading to a biased mean.

In situations where outliers are present, it's often advisable to use alternative measures of central tendency such as the **Median or Mode**, which are more robust to the influence of outliers.


## Median (Physical Mid point of data)
   - The median is the middle value of a dataset when it is arranged in ascending order.
   - If the dataset has an odd number of observations, the median is the middle value. If it has an even number of observations, the median is the average of the two middle values.
   - In other words, the median is the value that separates the higher half from the lower half of the data.
   - The median is less sensitive to extreme values (outliers) than the mean, making it a useful measure of central tendency when the data contains outliers or is skewed.

### Mean vs Median
- The mean is a measure of central tendency that represents the balance point or center of mass of the dataset, while the median represents the middle value of the dataset.
- The mean is sensitive to outliers and extreme values, while the median is more robust to outliers and provides a better measure of central tendency in skewed datasets.
- In symmetric distributions, the mean and median are equal. In skewed distributions, the mean may be pulled towards the direction of the skew, while the median remains unaffected.

*Both the Mean and Median provide measures of central tendency, they may give different insights into the typical value of a dataset depending on its distribution and the presence of outliers and often useful to consider both the mean and median when analyzing data to gain a comprehensive understanding of its central tendency.**

## Mode
   - The mode is the value that appears most frequently in the dataset.   
   - Unlike the mean and median, which require numerical data, the mode can be calculated for both numerical and categorical data.
   - The mode provides insight into the most common or typical value in the dataset.
   - In a frequency distribution, the mode corresponds to the peak of the distribution.
   - The mode is less affected by outliers or extreme values compared to the mean.
   - The mode can be useful for categorical data or when identifying the most common category in a frequency distribution.


Consider the following dataset representing the scores of students on a test:
{75,80,90,75,85,90,80,75,85,75}

In this dataset, the value 75 occurs most frequently (four times), making it the mode of the dataset.

The mode is particularly useful when dealing with categorical data or when identifying the most common value in a dataset. However, it may not always provide a comprehensive summary of the data, especially if the dataset has multiple modes or if the distribution is skewed. Therefore, it is often used in conjunction with other measures of central tendency, such as the mean and median, to gain a more complete understanding of the dataset.

If a dataset has no repeated values (i.e., all values occur only once), it is said to have no mode. A dataset can have one mode (unimodal), two modes (bimodal), or more than two modes (multimodal).

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/3b4b0b07-b8ff-41a8-8225-c2f0778ba2af)


These measures provide different perspectives on the central tendency of a dataset and are used depending on the nature of the data and the specific goals of the analysis.
