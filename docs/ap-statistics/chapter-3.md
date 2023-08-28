# Chapter 3: Numerical Methods for Describing Data Distributions

## Terms Definitions

Sample mean $\bar{x}$: Average from sample

Population mean $\mu$: Average from population

Median: Middle number

Interquartile Range: (3rd quartile - 1st quartile). Otherwise known as the range of the middle 50% of data

Population Standard Deviation $\sigma$: The average deviation from the mean

Population Variance is $\sigma^2$

$$
\sigma=\sqrt{\frac{\Sigma(x-\bar{x})^2}{n-1}}
$$

## Interpretations

The mean value of (# with unit) represents the typical value of (variable name)

The standard deviation (# with unit) is the amount on average, the values of (variable name with measurement) deviate from the mean. This indicates (high/low) variability

The median values of (# with unit) indicates that 50% of the data is above (# with unit) and 50% of the data is below (# with unit)

The IQR of (# with unit) is the range of the middle 50% of the data

## Box Plots

In statistics there are two types of centers that one may choose to use: sample mean $\bar{x}$, or median

A box plot must describe the minimum value, quartile 1, median, quartile 3, and max.

### Guessing Median Values

When $\int_a^bB(x)dx=\int_b^cB(x)dx$, the median exists at $b$

## Outliers

An outlier $x$ will exist under the following conditions

$$
x>Q_3+1.5IQR \text{ or } x<Q_1+1.5IQR
$$

!!! warning
    It is important to note that it is only greater or less than. Equal to does not constitute to an outlier

## Normal Curves

Normal curves are unimodal, symmetrical distributions, oftentimes referred to as a bell curve. The area under the curve is typically used to represent distributions.

### Empirical Rule

$$
(-\sigma, \sigma) \approx 68\%
\\\
(-2\sigma, 2\sigma) \approx 95\%
\\\
(-3\sigma, 3\sigma) \approx 99.7\%
$$

### z-scores

Describes the number of standard deviations $\sigma$ a value is above or below a mean data point

$$
z=\frac{x-\mu}{\sigma}
$$

#### Percentiles

The $n$th percentile is defined as the number where $n\%$ of the data is below. Keep in mind that high percentile isn’t always ideal

### Standard Normal Curve

The standard normal curve is when $\mu=0$ and $\sigma = 1$

Normalizing data is using the same index of the standard normal curve to find percentile