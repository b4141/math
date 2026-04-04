# Normal Distribution

# Definition

The normal distribution is a descriptive model that describes real world situations.

It is defined as a continuous frequency distribution of infinite range.

# Importance

Many dependent variables are commonly assumed to be normally distributed in the population

If a variable is approximately normally distributed we can make inferences about values of that variable.

# Characteristics

Bell-Shaped

Symmetry around the Mean $\mu$

$$
\mu = \frac{1}{n} \sum_{i=1}^{n}x_i
$$

Curve is asymptotic to the x-axis

Total area under the curve above the x-axis is 1 or 100%

The spread of the function is determined by the Standard Deviation $\sigma$

$$
\sigma = \sqrt{\frac{1}{n} \sum_{i=1}^{n}(x_i - \mu)^2}
$$

# Empirical Rule

68% of values lie within 1 standard deviation

95% within 2 standard deviations

99.7% within 3 standard deviations

# Mathematical Function *(PDF)*

This function is called the **Probability Density Function *(PDF)***

$$
f(x) = \frac{1}{\sqrt{2\pi\sigma^2}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}
$$

- $\pi$ = 3.14159
  
- $e$ = 2.61828
  
- $\mu$ : is the mean, the center of the bell shaped curve.
  
- $\sigma$ : standard deviation, the spread of the bell shape.
  

# The Standard Normal Distribution (Z)

$$
z = \frac{x-\mu}{\sigma}
$$

The Z-Score tells you how many standard deviations $\sigma$ a certain data point is away form the mean $\mu$

We standardize the data so we have a mean of 0 $\mu = 0$ and a standard deviation of 1 $\sigma = 1$

- The Mean $\mu$ = 0
  
- Standard Deviation $\mu = 1$
  

## Why standardize the data

- Enables fair comparisons
  
  - It allows you to compare scores from different groups. For example, you can determine if a student did better on a "hard" math test (mean 60) than an "easy" history test (mean 85) by seeing which z-score is higher.
    
- Prevents scale dominance
  
  -  If you are comparing "Age" (0–100) and "Annual Income" ($0–$100k+), the income values will mathematically "bully" the age values because they are much larger. Z-scores put them on a level playing field.
    
- Improves model convergences
  
  - Models such as that of neural networks converge faster when data is standardized
    
- Outlier Detection
  
  - Because standardized data follows a set scale, any value with a z-score greater than +3 or less than -3 is typically flagged as an unusual **outlier**.
    

## Probabilities are the areas under the curve

We use the Z-table which is a **lookup chart**, to find the area under the curve to the left.

![](https://cdn1.byjus.com/wp-content/uploads/2017/09/word-image2.png)

Example: for $z=1.25$ we get $P(Z<1.25) = 0.8944$

To get the probability of $P(Z>1.25)$ we subtract that from $1$ since the total area under the curve is $1$.
