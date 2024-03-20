# Fourier Series (Part 4)

## Changing the Interval for Fourier Approximations

!!! note
    All graphing pictures can be done on Desmos or another online graphing calculator. However, please show work on determining coefficients or any other work required.

Previously, we determined a Fourier series on the interval $[-\pi, \pi]$, which led to many things being zero and simplified our calculations. This interval implied that we wanted to model a function that had a period of $2 \pi$, which is not obviously always the case.

In this part, we want to change the interval to $[c, d]$. If this is the case, we need to make some changes to the sine and cosine terms. Since the period is changing now to $d-c$, we want to make the period of the sine and cosine terms to match, so we use $\beta = \frac{2 \pi}{d-c}$, which will lead to a Fourier series being of the form

$$ F(x) = a_0 + a_1 \cos(\beta x) + b_1 \sin(\beta x) + a_2 \cos(2 \beta x) + b_2 \sin(2 \beta x) + \cdots$$