# Skewness
Skewness is a measure of the asymmetry of the distribution of values in a dataset. It indicates whether the data is symmetrically distributed or if it tends to lean to one side.

![image](https://github.com/sateeshfrnd/Statistics/assets/8160366/ea80512e-b848-444c-9a0c-30f2d6cc012a)

Imagine a histogram or a line graph representing the data: if it slopes more to the right, it's right-skewed; if it slopes more to the left, it's left-skewed. Skewness helps us understand the shape and balance of the data distribution.

## No skewness
If the distribution is symmetric, it means it's evenly balanced around its central point, and the skewness is close to zero.

**(Mean = Median = Mode)**

## Positive skewness (right-skewed)
It indicates that the tail on the right side of the distribution is longer or stretched out, meaning there are some high values that pull the mean to the right. 

**(Mean >= Median >= Mode)**

Example:
- Distribution of marks in difficult Exam.
- Distribution of salary in a company.  

Outliers can contribute to positive skewness in a dataset because they pull the mean of the data towards the direction of their extreme values.

### Example, 
#### Distribution of students age
consider a dataset representing the ages of students in a class. Most students may be between 18 and 22 years old, but there might be a few older students who are outliers, say 30 years old or above. These outliers, being significantly older than the majority of students, would pull the mean age towards the higher end, resulting in a right-skewed distribution.

#### Distribution of companies profits
Similarly, in financial data, if a dataset represents the profits of companies, most companies may have moderate profits, but there could be a few companies with exceptionally high profits (outliers). These high-profit outliers would cause the distribution to be right-skewed because they contribute to a longer right tail.

*In summary, outliers with values larger than the majority of the data points can cause positive skewness by stretching the distribution towards the right side.*

## Negative skewness (left-skewed)
It indicates that the tail on the left side of the distribution is longer, implying there are some low values that pull the mean to the left.

**(Mode >= Median >= Mean)**

### Example
- Distribution Death Rates :- Death Rate is high after age 50
- Distribution of marks in easy exam :- very few students will fail
- Wealth distibution of the country :- very few people having good wealth.

## Data Distributional characteristics 
### Fairly Symmetric
If a distribution is "fairly symmetric," it means that it's balanced and doesn't show a strong tendency to lean to one side or the other. In this case, the skewness of the distribution would be close to zero, indicating minimal asymmetry.

**(-0.5 > 0 < 0.5)**

Imagine a histogram or a line graph representing the data: if it looks roughly the same on both sides of its central point, with no noticeable leaning towards the left or right, it's fairly symmetric.

Examples:
- Heights of adult males in a population where most heights cluster around the mean height, with relatively few extremely tall or short individuals.
- IQ scores in a large sample of individuals, where most scores are clustered around the mean IQ, with only a small number of exceptionally high or low scores.
- Ages of individuals in a community where most people are of middle age, with relatively few young or elderly outliers.

In summary, a distribution is fairly symmetric when it's reasonably balanced and doesn't show a significant skew towards one side.

### Moderatly Skewed
A moderately skewed distribution is one where there is noticeable asymmetry, but it's not extreme. In a moderately skewed distribution, the tail on one side of the distribution is longer or heavier than the other, indicating a tendency for the data to lean towards that side.

**(-1 ~ -0.5 & 0.5 ~ 1)**

1. **Positive Skewness (Right-Skewed)**: In a moderately right-skewed distribution, most of the data points are concentrated on the left side of the distribution, with a tail extending to the right. This suggests that there are some high values or outliers that pull the mean towards the right. Examples include income distribution in a population where a few individuals have significantly higher incomes than the majority.

2. **Negative Skewness (Left-Skewed)**: In a moderately left-skewed distribution, most of the data points are concentrated on the right side of the distribution, with a tail extending to the left. This suggests that there are some low values or outliers that pull the mean towards the left. An example might be the distribution of house prices in a city, where most prices are relatively high but a few properties are sold at much lower prices.

In summary, a moderately skewed distribution indicates that there is some degree of asymmetry, but it's not extreme. There is a noticeable tail on one side of the distribution, but it's not so heavy as to drastically affect the overall shape of the distribution.

### Highly Skewed
A highly skewed distribution is one where there is pronounced asymmetry, with a long tail extending prominently in one direction. This skewness indicates a significant imbalance in the distribution of values.

**(-1< & > +1)**

1. **Positive Skewness (Right-Skewed)**: In a highly right-skewed distribution, the majority of data points are concentrated on the left side of the distribution, with a long tail extending to the right. This indicates the presence of numerous high values or outliers that pull the mean towards the right. Examples include income distribution in a population where a small percentage of individuals earn exceptionally high incomes compared to the rest.

2. **Negative Skewness (Left-Skewed)**: In a highly left-skewed distribution, the bulk of data points are concentrated on the right side of the distribution, with a long tail extending to the left. This suggests the existence of numerous low values or outliers that pull the mean towards the left. For instance, the distribution of prices for luxury goods might be highly left-skewed, with most prices being high but a few outliers sold at significantly lower prices.

In summary, a highly skewed distribution indicates a significant imbalance in the data, with a long tail stretching prominently in one direction, either to the right or left. This skewness can have important implications for data analysis and interpretation.

## Visualizations 
Visualizations such as **histograms, box plots, density plots, QQ plots, and violin plots** are effective tools for quickly identifying skewness and distributional characteristics in a dataset. These visualizations provide insights into the shape, symmetry, and skewness of the data, guiding analytical decisions and interpretations.

## Handle Skewness
Handling data skewness is an important step in data preprocessing to ensure accurate analysis and modeling. 

Here are some common approaches to handle data skewness:
- **Transformations**: Apply mathematical transformations to the skewed variables to make their distributions more symmetrical. Common transformations include logarithmic, square root, and reciprocal transformations. These transformations can help reduce the impact of extreme values and make the data more suitable for parametric analysis.
- **Box-Cox Transformation**: The Box-Cox transformation is a family of power transformations that can stabilize the variance and make the data distribution more symmetric. It involves finding the optimal transformation parameter (lambda) that maximizes the log-likelihood of the data.
- **Treat the Outliers**:Replace extreme values (outliers) with less extreme values to mitigate their influence on the distribution. Winsorization involves setting the extreme values to a specified percentile of the data distribution, such as the 95th or 99th percentile.

## Summary
Understanding the concepts of skewness and the different types of distributions (symmetric, positively skewed, negatively skewed) is essential for several reasons:

1. **Interpreting Data**:
   - Skewness provides valuable insights into the shape and characteristics of a dataset.
   - It helps analysts understand whether the data is evenly distributed or if there are outliers or extreme values influencing the distribution.

2. **Data Analysis**:
   - Skewed distributions can affect the choice of statistical methods and techniques used for data analysis.
   - For instance, parametric tests like t-tests and ANOVA assume normality, so skewed data may require transformation or the use of non-parametric tests.

3. **Modeling**:
   - Skewness can impact the performance of predictive models.
   - Models trained on highly skewed data may not generalize well to new data, leading to biased predictions.
   - Understanding skewness can help in selecting appropriate modeling techniques and preprocessing steps.

4. **Decision-Making**:
   - Skewed data can influence decision-making processes in various domains, such as finance, healthcare, and marketing.
   - By understanding skewness, decision-makers can better interpret data trends, identify potential risks or opportunities, and make informed decisions.

5. **Communicating Results**:
   - Skewness is often reported in research papers, business reports, and presentations to provide a comprehensive understanding of the data.
   - Communicating skewness allows stakeholders to grasp the distributional characteristics of the data and the implications for decision-making.

In essence, understanding skewness and distributional characteristics is fundamental for accurate data analysis, effective decision-making, and clear communication of results in various fields and industries.

