# Series Methods and Tests

## Direct Comparison
Can be used to determine if a series converges or diverges by comparing it to a known series.

A function smaller than a convergent series will always converge, likewise, a function larger than a divergent series will always diverge.

!!! abstract "Direct Comparison Test"

    $$\text{If } a_n \leq b_n \text{ and } \sum_{n=1}^{\infty} b_n \text{ converges, then } \sum_{n=1}^{\infty} a_n \text{ converges.}$$

    $$\text{If } b_n \leq a_n \text{ and } \sum_{n=1}^{\infty} b_n \text{ diverges, then } \sum_{n=1}^{\infty} a_n \text{ diverges.}$$

!!! success "Conditions"
* $a_n$ and $b_n$ are both positive for all $n$.

## Limit Comparison
When a series is too difficult to compare directly, it can be compared to a similar known series that is easier to compare.

!!! abstract "Limit Comparison Test"

    $$\text{Given } \sum_{n=1}^{\infty} a_n \text{ and } \sum_{n=1}^{\infty} b_n \text{, let } c = \lim_{n \to \infty} \frac{a_n}{b_n}$$

    $$\text{If } c \text{ is a finite number} \newline \text{Then } \sum_{n=1}^{\infty} a_n \text{ and } \sum_{n=1}^{\infty} b_n \text{ either both converge or both diverge.}$$

!!! success "Conditions"
* $a_n$ and $b_n$ are both positive for all $n$.

## $p$-series
If a series follows the general form of a $p$-series, it can be determined if it converges or diverges.

!!! abstract "$p$-series"

    $$\text{If } \sum_{n=1}^{\infty} \frac{1}{n^p} \text{, then}$$

    $$\text{If } p > 1 \text{, then the series converges.} \newline \text{If } p \leq 1 \text{, then the series diverges.}$$

## Geometric Series

### Conditions
$f(x)$ is a geometric series if it follows the form $f(x) = ar^x$

## Telescopic Series

## Integral Test

## Test for Divergence

The series is divergent if

$$
\lim_{n \to \infty} a_n \neq 0
$$

## Ratio Test

## Root Test

## Alternating Series Test

### Conditions
$f(x)$ is an alternating series if it follows the form $f(x) = (-1)^n a_n$


