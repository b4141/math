```
https://www.youtube.com/watch?v=3VYupIsbLlY
https://www.youtube.com/watch?v=xlxaa9YhT6A
https://www.youtube.com/watch?v=xI9ZHGOSaCg
```

the x-axis represents the input

the y-axis represents the likelihood

normal distribution looks like bell curve, that's why it's often called a bell curve
this curve is centered around the distribution mean (μ) and spreads out with decreasing probability as you move away in either direction, although it's technically continues indefinitely in either direction, it only has significant probability value between 3 standard deviations (σ) bellow and above the mean.
-3σ -2σ -1σ μ +1σ +2σ +3σ.
between -1σ and +1σ there is 68% of the distribution data.
between -2σ and +2σ there is 95% of the data.
between -3σ and +3σ there is 99.7% of the data.

this distribution is so popular cause it can be used in so many types of applications.
example heights, weights, IQ follow a normal distribution very closely.
but each application comes with it own mean, standard deviation, and units.
this causes some problems, to solve this issue the units is often standardized (standardizing the data).
taking the original distribution and transfer it to have a mean of (0) and standard deviation of (1).
as a result any normal distribution of any magnitude are unit type can be converted to be centered
around (0) and extend more or less from (-3) to (+3).
-3 -2 -1 0 +1 +2 +3.

# How to standardize the data:

using the (Z-score)
z = (x-μ)/σ
this Z-score tells how many standard deviations (σ) a certain data point is away from the mean (μ).

example Heights of a group of people in a stack class were normally distributed with a
mean of μ = 66in
standard deviation of σ = 2in
then unstandardized distribution will look like this:
60 62 64 66 68 70 72
 μ

if x = 67 then z_x = (67 - 66)/2 = 0.5

so the **Z-Score** tells you how many standard deviations $\sigma$ a value is away from the mean.

$$
z = \frac{x-\mu}{\sigma}
$$

once you have the *Z-Score* you can use a function called The **Cumulative Distribution Function *(CDF)***.

The **CDF** gives you the area under the bell curve to the left of the point.

in other words it calculates the area for you.

if you want the area to the right which express the probability of being more, then just subtract the **CDF** value from 1 since the total area under the curve is 1

so the **Z-Score** gives you a point on the curve, and the **CDF** gives you the total probability to that point.

# Probability

calculate the mean using this formula:

$$
\mu = \frac{1}{n} \sum_{i=1}^{n}x_i
$$

calculating the standard deviation using this formula:

$$
\sigma = \sqrt{Variance}
$$

Where the $Variance$ is the average square distance from the mean:

$$
Variance = \frac{1}{n} \sum_{i=1}^{n}(x_i - \mu)^2
$$

### Variance vs Standard deviation

The variance gives us an intuitive way to measure spread, and insure that all values are positive

But the complication sits in the units, if the data is in **$cm$** then the variance is in **$cm^2$**, which makes data harder to interpret.

Taking the square root, gives us the standard deviation, a number that still reflects the spread but it's in the same units as the original data.

## Formula of the normal distribution:

This function is called the **Probability Density Function *(PDF)***

$$
f(x) = \frac{1}{\sqrt{2\pi\sigma^2}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}
$$

The **PDF** function gives the curve shape

use The **PDF** to calculate the probability that a value falls in a certain range.

The probability that a value lies between two numbers $A$ and $B$ is the area under the curve from $A$ tp $B$

![](file://C:\Users\HABIB\Documents\assets\2026-04-02-14-46-44-image.png?msec=1775311733570)

This requires calculus, most calculators have built in functions for working with the normal distribution.

The previous fig tells why it's called: The Probability Density Function

Think about how we talk about density in physics

$$
Density = \frac{Mass}{Volume}
$$

Density tells you how much matter is packed into a space, but you never ask how much matter is at a single point, instead you ask how much matter is in a region.

it's the same idea here, at a single point the probability is zero, what matters is the total probability across an interval.

---

uses:
outlier removal
outlier: is a data point which has a value that is very diffrent from the avrage values
may occure due to an error
treating by removal or applying some kind of transformation
formula to remove outlires:
