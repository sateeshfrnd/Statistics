# Geometric Mean

The geometric mean is a measure of central tendency that is calculated by taking the nth root of the product of n numbers. It is commonly used for quantities that exhibit multiplicative growth, such as investment returns, population growth rates, or ratios.

Calculate the geometric mean, multiply all the numbers together and then take the nth root, where n is the total number of values.

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/fed0a13a-f844-4294-8176-9b8daaebe304)


- The geometric mean is useful when dealing with quantities that have multiplicative relationships or when comparing growth rates over time.
- It is less sensitive to extreme values (outliers) compared to the arithmetic mean, making it suitable for skewed data distributions.
- It is commonly used in finance for calculating the average rate of return on investments over multiple periods.
- When dealing with percentages or ratios, the geometric mean preserves the same unit of measurement as the original values.
- The geometric mean is always equal to or less than the arithmetic mean.
- If any of the values in the dataset are zero, the geometric mean will also be zero.

## Example:

Consider a dataset representing the growth rates of three investments over three years:
{1.05,1.10,0.95}

```
Geometric Mean= 3√(1.05 X 1.10 X 0.95) = 3√1.068 ≈ 1.028

Percentage Growth Rate=(1.0275−1)×100=0.0275×100=2.75%
```

The geometric mean is a multiplicative average, so to convert it to a percentage growth rate, you can subtract 1 from the result and then multiply by 100 to get the percentage.


So, the percentage growth rate represented by the geometric mean of 1.0275 is indeed 2.75%.

In this example, the geometric mean growth rate over the three years is approximately 2.75%.

The geometric mean is a valuable tool for summarizing data with multiplicative relationships and is particularly useful in fields such as finance, biology, and ecology.

## Another Example:
Consider an example having camera dataset with details with zoom and review, as a data scientist which camera will buy with these data points.

```
Camera	    Zoom 	Review Score
Camera A	 200	  8
Camera B	 250	  6
```

Here, if we interpret "buying decision" as choosing the camera with the highest combined score (zoom and review), we could calculate a combined score for each camera using the geometric mean.

Geometric Mean for Camera A= √(200 X 8) = 40
Geometric Mean for Camera B= √(250 X 6) = 38

Choose the camera with the highest geometric mean score. In this case, Camera A have the same highest score.

**Geometric Mean is used when we want to compare two different properties.**



