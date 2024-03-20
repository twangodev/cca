# Fourier Series (Part 3)

## Taylor vs. Fourier Series Approximations

We are now going to compare the Taylor approximations and Fourier approximations to the same function to see which is better for approximating values.

Consider the function $f(x)=e^{-x^2}$

1. Write down the first four terms and the general term for the MacLaurin power series of $f(x)$. What is the interval of convergence?

    $$
    \begin{align}
    f(0) &= 1 \\
    f'(x) &= 0 \\
    f''(x) &= -2 \\
    f'''(x) &= 0 \\
    f^{(4)}(x) &= 12 \\
    f^{(6)}(x) &= -120 \\
    \end{align}
    $$

    $$
    \begin{align}
    f(x) &= 1 - \frac{2x^2}{2!} + \frac{12x^4}{4!} - \frac{120x^6}{6!} + \cdots \\
    &= 1 - x^2 + \frac{x^4}{2} - \frac{x^6}{6} + \cdots \\
    e^{-x^2} &= \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n}}{n!}
    \end{align}
    $$

    The interval of convergence is $(-\infty, \infty)$.

2. Let $T_n(x)$ be the $n$th degree Taylor series approximation for $f(x)$. Draw a graph of $f(x)$ and $T_2(x)$ on the same axes on the interval $[-\pi, \pi]$. How good of an approximation is $T_2(x)$ near zero? Near $\pi$?

    <iframe src="https://www.desmos.com/calculator/p1p5rfbc6q?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

    As the values approach 0, the approximation becomes more accurate. However, as the values approach $\pi$, the approximation becomes less accurate.

3. Let $F_n(x)$ be the Fourier series that goes up to the $nth$ term/coefficient. For example, $F_2(x) = a_0 + a_1 \cos(x) + b_1 \sin(x) + a_2 \cos(2x) + b_2 \sin(2x)$. Using your previous work on Fourier series, find the coefficients for $F_2(x)$. Graph $F_2(x)$ and $f(x)$ on the same axes on the interval $[-\pi, \pi]$. How good of an approximation is $F_2(x)$ near zero? Near $\pi$?

    <iframe src="https://www.desmos.com/calculator/jpywezfdq9?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

    As the values approach 0, the approximation yields an underestimation. However, as the values approach $\pi$, the approximation yields an overestimation. The approximation around $\pi$ is much better than the previous Taylor Series approximation.

Now we will define something called the least-squares error, which takes the form of $\int_a^b(g_1(x) - g_2(x))^2dx$. The argument in parentheses represents the difference between the actual function and its approximation. Think about why this would be called the "least-squares error."

1. Find the least squares error for $T_4(x)$, $T_6(x)$, and $T_8(x)$.

    $$
    \begin{align}
    T_4(x) &= 1 - x^2 + \frac{x^4}{2} - \frac{x^6}{6} \\
    T_6(x) &= 1 - x^2 + \frac{x^4}{2} - \frac{x^6}{6} + \frac{x^8}{24} \\
    T_8(x) &= 1 - x^2 + \frac{x^4}{2} - \frac{x^6}{6} + \frac{x^8}{24} - \frac{x^{10}}{120} \\
    \end{align}
    $$

    $$
    \begin{aligned}
    E_4 &= \int_{-\pi}^{\pi}(f(x)-T_4(x))^2dx &= 6416.169 \\
    E_6 &= \int_{-\pi}^{\pi}(f(x)-T_6(x))^2dx &= 25822.818 \\
    E_8 &= \int_{-\pi}^{\pi}(f(x)-T_8(x))^2dx &= 71126.021 \\
    \end{aligned}
    $$

2. Explain why we would expect the least squares error to increase for $T_{2k}$ as $k$ increases (at least for some time)

    The least squares error increases for $T_{2k}$ as $k$ increases because the Taylor series approximation becomes less accurate as the degree of the polynomial increases. This is because the Taylor series is only accurate near the point of expansion, and as the degree increases, the approximation becomes less accurate

3. Find the least squares error for $F_3(x)$, $F_4(x)$, and $F_5(x)$.

    $$
    \begin{aligned}
    a_0 = \int_{-\pi}^{\pi}e^{-x^2}dx &= 0.28209 \\
    a_1 = \int_{-\pi}^{\pi}e^{-x^2}\cos(x)dx &= 0.43939 \\
    b_1 = \int_{-\pi}^{\pi}e^{-x^2}\sin(x)dx &= 0 \\
    a_2 = \int_{-\pi}^{\pi}e^{-x^2}\cos(2x)dx &= 0.20754 \\
    b_2 = \int_{-\pi}^{\pi}e^{-x^2}\sin(2x)dx &= 0 \\
    a_3 = \int_{-\pi}^{\pi}e^{-x^2}\cos(3x)dx &= 0.0594 \\
    b_3 = \int_{-\pi}^{\pi}e^{-x^2}\sin(3x)dx &= 0 \\
    a_4 = \int_{-\pi}^{\pi}e^{-x^2}\cos(4x)dx &= 0.0103 \\
    b_4 = \int_{-\pi}^{\pi}e^{-x^2}\sin(4x)dx &= 0 \\
    a_5 = \int_{-\pi}^{\pi}e^{-x^2}\cos(5x)dx &= 0.00109 \\
    b_5 = \int_{-\pi}^{\pi}e^{-x^2}\sin(5x)dx &= 0 \\
    \end{aligned}
    $$

    $$
    \begin{align}
    F_3(x) &= 0.28209 + \cdots + 0.0594\cos(3x) \\
    F_4(x) &= 0.28209 + \cdots + 0.0594\cos(3x) + 0.0103\cos(4x) \\
    F_5(x) &= 0.28209 + \cdots + 0.0594\cos(3x) + 0.0103\cos(4x) + 0.00109\cos(5x) \\
    \end{align}
    $$

    $$
    \begin{aligned}
    E_3 &= \int_{-\pi}^{\pi}(f(x)-F_3(x))^2dx &= 0.0003389 \\
    E_4 &= \int_{-\pi}^{\pi}(f(x)-F_4(x))^2dx &= 0.00000376 \\
    E_5 &= \int_{-\pi}^{\pi}(f(x)-F_5(x))^2dx &= 1.416 \times 10^{-8} \\
    \end{aligned}
    $$

4. Explain why we would expect the least squares error to decrease for $F_k(x)$ as $k$ decreases.

    The least squares error decreases for $F_k(x)$ as $k$ decreases because the Fourier series approximation becomes more accurate as the number of terms in the series increases. This is because the Fourier series is accurate over the entire interval, and as the number of terms increases, the approximation becomes more accurate.

5. For what value of $k$ does the least squares error of $T_k(x)$ first become less than 0.001? Show your work. (This is in contrast to #5, to show that eventually error can become smaller)

    $$ E_k = \int_{-\pi}^{\pi}\left(f(x)- \sum_{n=0}^{k} \frac{(-1)^n x^{2n}}{n!} \right)^2dx $$

    <iframe src="https://www.desmos.com/calculator/lxazgvn9xo?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

    | $k$      | $E_k$                   |
    |----------|-------------------------|
    | 2        | 1001.0305               | 
    | 3        | 6416.1698               | 
    | $\cdots$ | $\cdots$                |
    | 23       | 0.0463                  |
    | 24       | 0.007                   |
    | 25       | 0.001                   |
    | 26       | 1.3145 \times 10 ^ {-4} |

    The least squares error of $T_{26}(x)$ first becomes less than 0.001.

6. For what value of $k$ does the least squares error of $F_k(x)$ first become less than 0.00001? Show your work.

    The least squares error of $F_4(x)$ is already less than 0.00001. See #3.