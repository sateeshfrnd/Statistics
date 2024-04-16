# Kurtosis
Kurtosis is a statistical measure that quantifies the "tailedness" of a probability distribution, indicating how sharply peaked or flat the distribution is compared to a normal distribution. 

It measures whether the data is heavy-tailed or light-tailed in a normal distribution.

Kurtosis refers to the degree of presence of outliers (extreme values) in the distribution.

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/a2cfb4c7-2653-492f-bffa-79ab55ef6dac)

## Peakedness:
- Kurtosis measures the height and sharpness of the central peak of a distribution.
- A high kurtosis value indicates a distribution with a sharp peak (more data points clustered around the mean), while a low kurtosis value indicates a distribution with a flatter peak (fewer data points near the mean).

## Tails:
- Kurtosis also describes the tails of the distribution, which are the regions away from the center (mean) of the distribution.
- A high kurtosis value indicates heavy tails, where there are more extreme values in the distribution compared to a normal distribution.
- A low kurtosis value indicates light tails, where there are fewer extreme values compared to a normal distribution.

# Types of excess kurtosis
The excess kurtosis is used in statistics and probability theory to compare the kurtosis coefficient with that normal distribution. Excess kurtosis can be positive (Leptokurtic distribution), negative (Platykurtic distribution), or near to zero (Mesokurtic distribution).

Since normal distributions have a kurtosis of 3, excess kurtosis is calculating by subtracting kurtosis by 3.

**Excess kurtosis  =  Kurt – 3**

### 1. Mesokurtic (kurtosis = 3)
A distribution with a kurtosis value equal to 3 is said to be Mesokurtic, indicating that its shape is similar to that of a normal distribution.

**Excess kurtosis in Mesokurtic = 3-3 = 0**

### 2. Leptokurtic (kurtosis > 3)
Leptokurtic is having very long and skinny tails, which means there are more chances of outliers. Positive values of kurtosis indicate that distribution is peaked and possesses thick tails. An extreme positive kurtosis indicates a distribution where more of the numbers are located in the tails of the distribution instead of around the mean.

### 3. Platykurtic (kurtosis < 3)
Platykurtic having a lower tail and stretched around center tails means most of the data points are present in high proximity with mean. A platykurtic distribution is flatter (less peaked) when compared with the normal distribution.

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/88f57e40-1fdb-4906-94b8-145964ace527)

## Interpretation
- Understanding the kurtosis of a distribution helps in identifying the shape and characteristics of the data.
- High kurtosis can indicate a distribution with outliers or heavy-tailed data, which may require special attention in data analysis.
- Low kurtosis can indicate a distribution with lighter tails, which may result in less extreme observations compared to a normal distribution.

## Summary
Kurtosis provides valuable information about the shape and tails of a distribution, enabling data scientists to better understand the characteristics of their data and choose appropriate statistical techniques for analysis.
