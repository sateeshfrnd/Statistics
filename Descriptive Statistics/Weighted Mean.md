# Weighted Mean

The weighted mean, also known as the weighted average, is a statistical measure that takes into account the importance, relevance, or frequency of each value in a dataset.

It is calculated by multiplying each value by its corresponding weight, summing these products, and then dividing by the sum of the weights.

Mathematically, the population weighted mean μ is calculated as:

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/1bb5df34-6f6f-4a6e-9398-ab0523a9499a)

Where:
- ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/99d7b8c0-4858-4921-8aa2-a6b50075ba78) represents the individual values in the population.
- ![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/d83483ef-529e-4a38-b1c7-7c409014cf24) represents the corresponding weights assigned to each value in the population.
- N is the total number of values in the population.

## Example

Suppose we have a population of cities, and we want to calculate the average population size of these cities, where each city's population is weighted by its relative importance (e.g., its contribution to the overall population of the region).

Here is the data for five cities:
```
City A: Population = 100,000, Weight = 0.2
City B: Population = 150,000, Weight = 0.3
City C: Population = 120,000, Weight = 0.1
City D: Population = 200,000, Weight = 0.25
City E: Population = 180,000, Weight = 0.15
```

Lets calculate the population weighted mean:
1. Multiply each city's population by its corresponding weight.
   ```
   City A weighted value= 100,000 × 0.2 = 20,000
   City B weighted value= 150,000 × 0.3 = 45,000
   City C weighted value= 120,000 × 0.1 = 12,000
   City D weighted value= 200,000 × 0.25 = 50,000
   City E weighted value= 180,000 × 0.15 = 27,000
   ```
2. Sum up the products obtained in step 1.
  ```
   Sum of weighted values = 20,000 + 45,000 + 12,000 + 50,000 + 27,000 =154,000
  ``` 
3. Divide the sum from step 2 by the total sum of weights.
```
Total sum of weights = 0.2+0.3+0.1+0.25+0.15=1

Population weighted mean= 154,000 / 1 = 154,000
```
So, the population weighted mean population size of these cities is 154,000.

## Summary
*Weighted Mean is particularly useful in situations where some values in a dataset are more important or have greater significance compared to others.* By assigning weights to each value based on their importance, relevance, or frequency, the weighted mean ensures that these differences are appropriately reflected in the calculation of the mean.

Examples:
- In a survey, responses from certain demographics or groups may be more representative of the population or of particular interest. Assigning higher weights to these responses ensures that they have a greater impact on the overall results.
- In financial analysis, the performance of assets in an investment portfolio may be weighted based on their allocation or contribution to the portfolio's overall return. Assets with higher weights have a larger influence on the portfolio's performance.
- When calculating average grades in a class, assignments or exams may be weighted differently based on their difficulty or importance in the curriculum. Assigning higher weights to more critical assessments ensures that they have a greater influence on the final grade.
  
In each of these scenarios, the weighted mean allows for a more nuanced analysis that takes into account the varying importance of different values, leading to more accurate and meaningful conclusions.
