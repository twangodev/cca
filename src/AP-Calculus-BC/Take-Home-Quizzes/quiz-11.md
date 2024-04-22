# Fourier Series (Part 4)

## Changing the Interval for Fourier Approximations

!!! note
    All graphing pictures can be done on Desmos or another online graphing calculator. However, please show work on determining coefficients or any other work required.

Previously, we determined a Fourier series on the interval $[-\pi, \pi]$, which led to many things being zero and simplified our calculations. This interval implied that we wanted to model a function that had a period of $2 \pi$, which is not obviously always the case.

In this part, we want to change the interval to $[c, d]$. If this is the case, we need to make some changes to the sine and cosine terms. Since the period is changing now to $d-c$, we want to make the period of the sine and cosine terms to match, so we use $\beta = \frac{2 \pi}{d-c}$, which will lead to a Fourier series being of the form

$$ F(x) = a_0 + a_1 \cos(\beta x) + b_1 \sin(\beta x) + a_2 \cos(2 \beta x) + b_2 \sin(2 \beta x) + \cdots$$

The terms that we found previously also need to be modified. The term $a_0$ will now be $\frac{1}{d-c} \int_{c}^{d} f(x) dx$. The terms for $a_k$ and $b_k$ are also modified to be

$$
a_k = \frac{2}{d-c} \int_{c}^{d} f(x) \cos(k \beta x) dx \quad \text{and} \quad b_k = \frac{2}{d-c} \int_{c}^{d} f(x) \sin(k \beta x) dx
$$

1. Consider the function $f(x) = 1- x^2$ on the interval $[0, 1]$. Determine the coefficients of the Fourier approximation of order 3 (i.e. $F_3(x)$). Graph $f(x)$ and the Fourier approximation on the same axes and compare them. Make sure to look at an expanded window to notice the periodicity.

    $$
    \begin{aligned}
    a_0 &= \frac{1}{1-0} \int_{0}^{1} (1-x^2) dx & \approx 0.6667\\
    a_1 &= \frac{2}{1-0} \int_{0}^{1} (1-x^2) \cos(\beta x) dx & \approx -0.1013\\
    b_1 &= \frac{2}{1-0} \int_{0}^{1} (1-x^2) \sin(\beta x) dx & \approx 0.3183\\
    a_2 &= \frac{2}{1-0} \int_{0}^{1} (1-x^2) \cos(2\beta x) dx & \approx -0.0253\\
    b_2 &= \frac{2}{1-0} \int_{0}^{1} (1-x^2) \sin(2\beta x) dx & \approx 0.1591\\
    a_3 &= \frac{2}{1-0} \int_{0}^{1} (1-x^2) \cos(3\beta x) dx & \approx -0.0112\\
    b_3 &= \frac{2}{1-0} \int_{0}^{1} (1-x^2) \sin(3\beta x) dx & \approx 0.1061\\
    \end{aligned}
    $$

    Within the interval $[0, 1]$:

    <iframe src="https://www.desmos.com/calculator/4yfzigkixg?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

    Expanded Window:

    <iframe src="https://www.desmos.com/calculator/6gy7txxomr?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

2. Now do the same thing as #1 for the function $f(x) = x$ on $[0, 1]$.

    $$
    \begin{aligned}
    a_0 &= \frac{1}{1-0} \int_{0}^{1} x dx & = 0.5\\
    a_1 &= \frac{2}{1-0} \int_{0}^{1} x \cos(\beta x) dx & = 0\\
    b_1 &= \frac{2}{1-0} \int_{0}^{1} x \sin(\beta x) dx & \approx -0.3183\\
    a_2 &= \frac{2}{1-0} \int_{0}^{1} x \cos(2\beta x) dx & = 0\\
    b_2 &= \frac{2}{1-0} \int_{0}^{1} x \sin(2\beta x) dx & \approx -0.1591\\
    a_3 &= \frac{2}{1-0} \int_{0}^{1} x \cos(3\beta x) dx & = 0\\
    b_3 &= \frac{2}{1-0} \int_{0}^{1} x \sin(3\beta x) dx & \approx -0.1061\\
    \end{aligned}
    $$

    Within the interval $[0, 1]$:

    <iframe src="https://www.desmos.com/calculator/nx63bspwas?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

    Expanded Window:

    <iframe src="https://www.desmos.com/calculator/qoexj7gh7d?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

3. Now we will consider a piecewise function. For the function $f(x) = \begin{cases} x + 1 & 0 \leq x \leq \frac{1}{2} \\ -x + 2 & \frac{1}{2} \leq x \leq 1 \end{cases}$ find the coefficients of the third-order Fourier approximation. Consider that this function will be repeating with a period of one. (Hint: Think of the period that we want, and also the interval of the function that we want to model. These two things are different, so you need to adjust the integrals to account for this). Graph $f(x)$ and $F_3(x)$ on the same axes.

    $$
    \begin{align}
    c = 0, \quad d = 1, \quad \beta = \tau = 2 \pi\\
    \end{align}
    $$

    $$
    \begin{aligned}
    a_0 &= \frac{1}{1-0} \int_{0}^{1} f(x) dx & = 1.25\\
    a_1 &= \frac{2}{1-0} \int_{0}^{1} f(x) \cos(\beta x) dx & \approx -0.2026\\
    b_1 &= \frac{2}{1-0} \int_{0}^{1} f(x) \sin(\beta x) dx & = 0\\
    a_2 &= \frac{2}{1-0} \int_{0}^{1} f(x) \cos(2\beta x) dx & = 0\\
    b_2 &= \frac{2}{1-0} \int_{0}^{1} f(x) \sin(2\beta x) dx & = 0\\
    a_3 &= \frac{2}{1-0} \int_{0}^{1} f(x) \cos(3\beta x) dx & \approx -0.0225\\
    b_3 &= \frac{2}{1-0} \int_{0}^{1} f(x) \sin(3\beta x) dx & = 0\\
    \end{aligned}
    $$

    <iframe src="https://www.desmos.com/calculator/dwvqkphrto?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

4. Now consider the piecewise function $f(x) = \begin{cases} 0 & 0 \leq x < \frac{3}{4} \\ 1 & \frac{3}{4} \leq x \leq 1 \end{cases}$. Repeat #3 with this function.

    $$
    \begin{align}
    c = 0, \quad d = 1, \quad \beta = \tau = 2 \pi\\
    \end{align}
    $$

    $$
    \begin{aligned}
    a_0 &= \frac{1}{1-0} \int_{0}^{1} f(x) dx & = \frac{1}{4}\\
    a_1 &= \frac{2}{1-0} \int_{0}^{1} f(x) \cos(\beta x) dx & \approx 0.3183\\
    b_1 &= \frac{2}{1-0} \int_{0}^{1} f(x) \sin(\beta x) dx & \approx -0.3183\\
    a_2 &= \frac{2}{1-0} \int_{0}^{1} f(x) \cos(2\beta x) dx & = 0\\
    b_2 &= \frac{2}{1-0} \int_{0}^{1} f(x) \sin(\beta x) dx & \approx -0.3183\\
    a_3 &= \frac{2}{1-0} \int_{0}^{1} f(x) \cos(3\beta x) dx & \approx -0.1061\\
    b_3 &= \frac{2}{1-0} \int_{0}^{1} f(x) \sin(3\beta x) dx & \approx -0.1061\\
    \end{aligned}
    $$

    <iframe src="https://www.desmos.com/calculator/9t6svg7gug?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

