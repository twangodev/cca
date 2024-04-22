# 6: Random Variables and Probability Distributions

## Random Variables

Random variables are defined as a variable that depends on the outcomes of a chance experiment, which are numerical values

### Types of Random Variables

#### Discrete

Variables which are measurable and countable

#### Continuous

Variables which can consist of any numeric value

### Properties of Probability Distributions

#### Expected Values and Standard Deviations

$$
E=\Sigma x\times p(x)\\
\sigma_x=\Sigma(x-\mu_x)^2p(x)
$$

## Linear Combinations

### Properties of Data Points

Let $x$ be any data point, and $c$ any constant

#### Addition and Subtraction

Represented by $x+c$

$$
\mu =\mu+c\\
\sigma=\sigma
$$

#### Multiplication and Subtraction

Represented with $xc$

$$
\mu=c\mu\\
\sigma=c\sigma
$$

### Variances and Standard Deviations

$$
\sigma^2=\Sigma\sigma^2\\
\therefore\sigma=\sqrt{\Sigma\sigma^2}
$$

## Distributions

### Binomial Distributions

Binomial distributions have two possibilities, most commonly true or false. $P(\text{success})$ must be constant every round, trials must be independent, and there are a finite amount of trials

$$
\mu_x=np\\
\sigma_x=\sqrt{np(1-p)}
$$

### Geometric Distributions

Geometric distributions have two possibilities, most commonly true or false. $P(\text{success})$ must be constant every round, trials must be independent, you keep going until first success. Geometric distributions must atleast have one trial

$$
P(x)=(1-P(s))^{n-1}P(s)\\
\mu_x=\frac{1}{p}\\
\sigma_x=\frac{\sqrt{1-p}}{p}
$$

### Normal Distributions

Combination of two normal distributions