# Convergence/Divergence Tests

## Test for Divergence
The series $\sum_{n=1}^{\infty} a_n$ diverges if $\lim_{n \to \infty} a_n \neq 0$. In other words, if the terms of the series do not approach zero, then the series is guaranteed to diverge.

!!! warning
    The test for divergence is a necessary but not sufficient condition for convergence. If the limit of the terms of the series is zero, then the series may or may not converge, and further tests are needed to determine convergence.

## Geometric Series Test
The geometric series $\sum_{n=0}^{\infty} ar^n$ converges if $|r| < 1$ and diverges if $|r| \geq 1$. 

!!! tip
    The sum of an infinite geometric series is $\frac{a}{1-r}$ if $|r| < 1$.

## p-Series Test
The p-series $\sum_{n=1}^{\infty} \frac{1}{n^p}$ converges if $p > 1$ and diverges if $p \leq 1$.

## Integral Test
The series $\sum_{n=1}^{\infty} a_n$ converges if the integral $\int_{1}^{\infty} f(x) \, dx$ converges, where $f(x) = a_x$.

## Direct Comparison Test
Given $\sum_{n=1}^{\infty} a_n$ and $\sum_{n=1}^{\infty} b_n$, if $0 \leq a_n \leq b_n$ for all $n$ and $\sum_{n=1}^{\infty} b_n$ converges, then $\sum_{n=1}^{\infty} a_n$ converges. 

Conversely, if $0 \leq a_n \leq b_n$ for all $n$ and $\sum_{n=1}^{\infty} a_n$ diverges, then $\sum_{n=1}^{\infty} b_n$ diverges.

## Limit Comparison Test
Given $\sum_{n=1}^{\infty} a_n$ and $\sum_{n=1}^{\infty} b_n$, if $\lim_{n \to \infty} \frac{a_n}{b_n} = c > 0$, then either both series converge or both series diverge.

## Alternating Series Test
The alternating series $\sum_{n=1}^{\infty} (-1)^{n-1}b_n$ converges **if and only if** the following conditions are met:

1. $b_{n+1} \leq b_n$ for all $n$. In other words, the terms of the series are monotonically decreasing.
2. $\lim_{n \to \infty} b_n = 0$. In other words, the terms of the series approach zero.

## Ratio Test
Given $\sum_{n=1}^{\infty} a_n$, if $\lim_{n \to \infty} \left| \frac{a_{n+1}}{a_n} \right| = L$, then:

- If $L < 1$, the series converges.
- If $L > 1$, the series diverges.
- If $L = 1$, the test is inconclusive.

## Root Test
Given $\sum_{n=1}^{\infty} a_n$, if $\lim_{n \to \infty} \sqrt[n]{|a_n|} = L$, then:

- If $L < 1$, the series converges.
- If $L > 1$, the series diverges.
- If $L = 1$, the test is inconclusive.


