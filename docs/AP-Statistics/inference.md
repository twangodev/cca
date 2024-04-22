# Statistical Inference Methods

## Proportional

### Confidence Interval

#### One Sample z-interval

Conditions:

- Random/Representative Sample
- Independent Samples
- Normality: $n\hat{p}\ge10$ and $n(1-\hat{p})\ge10$

$$
\hat{p} \pm z^\star\sqrt{\frac{\hat{p}(1-\hat{p})}{n}}

$$

Assuming the sample was selected in a reasonable manner, we are CLEVEL% confident that the actual proportion of VAR is between LOW and HIGH

#### Two Sample z-interval

- Both random/representative samples
- Both independent samples
- Normality on both samples: $n\hat{p}\ge10$ and $n(1-\hat{p})\ge10$

$$
(\hat{p}_1 - \hat{p}_2) \pm z^\star\sqrt{\frac{\hat{p}_1(1-\hat{p}_1)}{n_1} + \frac{\hat{p}_2(1-\hat{p}_2)}{n_2}}
$$

Assuming the sample was selected in a reasonable manner, we are CLEVEL% confident that the difference of proportions of VAR is between LOW and HIGH

### Hypothesis Tests

#### One Sample z-test

$$
h_0: p=p_0

\\

h_a:p>, \ne, < p_0
$$

Conditions

- Random/representative samples
- Independent samples
- Normality: $n \ge 30$

$$
z = \frac{\hat{p} - p_0}{\sqrt{\frac{p_0(1-p_0)}{n}}}
$$

Reject $h_0$ when the p-value is less than $\alpha$ (there is convincing evidence to support the alternative hypothesis), otherwise fail to reject (there lacks convincing evidence to support the alternative hypothesis).

#### Two Sample z-test

$$
h_0: p_1=p_2

\\

h_a:p_1>, \ne, < p_2
$$

Conditions

- Random/representative samples
- Independent samples
- Normality: $n \ge 30$

$$
\Large
\hat{p_c}=\frac{n_1\hat{p_1}+n_2\hat{p_2}}{n_1+n_2}
\\\\
z = \frac{\hat{p}_1 - \hat{p}_2}{\sqrt{\frac{\hat{p}_c(1-\hat{p}_c)}{n_1} + \frac{\hat{p}_c(1-\hat{p}_c)}{n_2}}}

$$

Assuming the sample was selected in a reasonable manner, we are CLEVEL% confident that the difference of proportions of VAR is between LOW and HIGH

## Mean

### Confidence Interval

#### One Sample t-interval

Conditions:

- Random/representative sample

$$
\bar{x} \pm t^\star\frac{s}{\sqrt{n}}
$$

#### Two Sample t-interval (dependent & paired)

$$
(\bar{x}_1 - \bar{x}_2) \pm t^\star \frac{s_d}{\sqrt{n}}

$$

#### Two Sample t-interval (independent)

$$
(\bar{x}_1 - \bar{x}_2) \pm t^* \sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}

$$

### Hypothesis Test

#### One Sample t-test

$$
t = \frac{\bar{x} - \mu_0}{\frac{s}{\sqrt{n}}}
$$

#### Two Sample t-test (dependent)

$$
t^\star = \frac{\bar{x_d}}{\frac{s_d}{\sqrt{n}}}
$$

#### Two Sample t-test (independent)

$$
t^\star = \frac{\bar{x}_1 - \bar{x}_2}{\sqrt{\frac{s_1^2}{n_1} + \frac{s_2^2}{n_2}}}
$$

## Power of Tests

P-Hat: Sample Proportion

P-Naught: Hypothesized Proportion

P: Population Proportion

P-Vale: Probability that you would observe p-hat or something more extreme if p-naught were true

Power of a test: Probability of h0 rejection when it is false or should be rejected $1-\beta$. Higher power indicates smaller beta. To increase power: Increase n (increases SE - curve gets skinner), or increase alpha (increases rejection zone)