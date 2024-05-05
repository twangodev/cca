# Integration Technique Review

1. $\int_1^2 (9x^2 - 4x + 1) \ln x \, dx$

    $$
    \begin{align}
    &= \int_1^2 9x^2 \ln x \, dx - \int_1^2 4x \ln x \, dx + \int_1^2 \ln x \, dx \\
    &= \left[ 3x^3 \ln x - \int 3x^2 \, dx \right]_1^2 - \left[ 2x^2 \ln x - \int 2x \, dx \right]_1^2 + \left[ x \ln x - x \right]_1^2 \\
    &= \left[ 3x^3 \ln x - x^3 \right]_1^2 - \left[ 2x^2 \ln x - x^2 \right]_1^2 + \left[ x \ln x - x \right]_1^2 \\
    &= \left[ 24 \ln 2 - 8 - 3 \ln 1 + 1 \right] - \left[ 8 \ln 2 - 4 - 4 \ln 1 + 1 \right] + \left[ 2 \ln 2 - 2 - \ln 1 + 1 \right] \\
    &= 24 \ln 2 - 8 - 3 + 1 - 8 \ln 2 + 4 + 4 - 1 + 2 \ln 2 - 2 - 1 + 1 \\
    &= 24 \ln 2 - 8 \ln 2 + 2 \ln 2 - 8 + 4 + 4 - 3 - 1 - 2 - 1 + 1 \\
    &= 18 \ln 2 - 7 \quad \blacksquare
    \end{align}
    $$

2. The function $f$ has a continuous derivative. The table below gives values of $f$ and its derivative for $x=0$ and $x=4$. If $\int_0^4 f(x) \, dx = 8$, what is the value of $\int_0^4 xf'(x) \, dx$?

    | $x$ | $f(x)$ | $f'(x)$ |
    |-----|--------|---------|
    | $0$ | $2$    | $5$     |
    | $4$ | $-3$   | $11$    |

    $$
    \begin{align}
    u = x \quad & dv = f'(x) \, dx \\
    du = dx \quad & v = f(x)
    \end{align}
    $$

    $$
    \begin{align}
    \int_0^4 xf'(x) \, dx &= \left[ x f(x) \right]_0^4 - \int_0^4 f(x) \, dx \\
    &= 4f(4) - 0f(0) - 8 \\
    &= 4(-3) - 0(2) - 8 \\
    &= -12 - 8 \\
    &= -20 \quad \blacksquare
    \end{align}
    $$

3. $\int x \sin(6x) \, dx$

    $$
    \begin{align}
    u = x \quad & dv = \sin(6x) \, dx \\
    du = dx \quad & v = -\frac{1}{6} \cos(6x)
    \end{align}
    $$

    $$
    \begin{align}
    \int x \sin(6x) \, dx &= -x \frac{1}{6} \cos(6x) - \int -\frac{1}{6} \cos(6x) \, dx \\
    &= -\frac{x}{6} \cos(6x) + \frac{1}{6} \int \cos(6x) \, dx \\
    &= -\frac{x}{6} \cos(6x) + \frac{1}{6} \left[ \frac{1}{6} \sin(6x) \right] \\
    &= -\frac{x}{6} \cos(6x) + \frac{1}{36} \sin(6x) + C \quad \blacksquare
    \end{align}
    $$

4. $x f(x) \, dx$

$$
\begin{align}
u = x \quad & dv = f(x) \, dx \\
\end{align}
$$


5. If $\int f(x) \sin x \, dx = - f(x) \cos x + \int 3x^2 \cos x \, dx$, then $f(x)$ could be
6. $\int_1^e x^4 \ln x \, dx$
7. $\int \frac{7x}{(2x-3)(x+2)} \, dx$
8. $\int \frac{1}{x^2 - 7x + 10} \, dx$
9. Which of the following expressions is equal to $\int_0^2 \frac{17x+4}{3x^2-7x-6} \, dx$?
10. $\int \frac{2x}{(x+2)(x+1)} \, dx$
11. Let $R$ be the region between the graph of $y=e^{-2x}$ and the $x$-axis for $x \geq 3$. The area of $R$ is
12. $\int_0^3 \frac{dx}{(1-x)^2}$
13. $\int_1^{\infty} xe^{-x^2} \, dx$
14. What are all values of $p$ for which $\int_1^{\infty} \frac{1}{x^{3p + 1}} \, dx$ converges?
15. An antiderivative of $\frac{e^x}{e^x - 1}$ is $\ln |e^x - 1|$. Which of the following statements about the integral $\int_{-2}^2 \frac{e^x}{e^x - 1} \, dx$ is true?
16. $\int_0^4 \frac{1}{\sqrt{x}(1+\sqrt{x})} \, dx$