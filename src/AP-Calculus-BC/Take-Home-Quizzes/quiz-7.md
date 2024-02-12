# Fourier Series (Part 1)
## Introduction and Derivation of Fourier Series

In our calculus class, we've studied using Taylor series. A Taylor series approximates a function by using derivatives at a specific point to generate a polynomial.

However, there is a different way to approximate a function called Fourier series, pioneered by Joseph Fourier in the early 1800's. What a Fourier series does is approximate a function using sines and cosines over an interval. It is useful in approximating complex periodic phenomena, such as heat flows, oscillations, vibrations, sound, and anything else that exhibits wave behavior. In a modern sense, we use it in musical analysis, speech recognition, and filtering of sound.

A Fourier series is an infinite trigonometric series of the form:

$$
F(x) = a_0 + a_1\cos{x} + b_1\sin{x} + a_2\cos{2x} + b_2\sin{2x} + a_3\cos{3x} + b_3\sin{3x} + \cdots
$$

This can be written using the summation notation as

$$
F(x) = \sum_{k=0}^{\infty} a_k\cos{kx} + b_k\sin{kx}
$$

To write a Fourier series, the goal is to find values of $a_{k}$ and $b_{k}$ to approximate a function $f(x)$.
Here is a picture of approximating the function $f(x)=e^{-x^{2}}$ using a second-order Fourier approximation.

<iframe src="https://www.desmos.com/calculator/g9x9aptg8n?embed" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

## Fourier Series for Even Functions

We will begin by looking at only even functions, which have the property $f(x)=f(-x)$, An even Fourier series, called $F_{e}(x)$ only has cosine terms (you should understand why...) and can be used to approximate the even function. Therefore,

$$
F_{e}(x) = a_0 + a_1\cos{x} + a_2\cos{2x} + a_3\cos{3x} + \cdots
$$

Assume we have some even function $f(x)$ that we want to look at on the interval $[-\pi,\pi]$. We want to find $F_{e}(x)$ such that $F_{e}(x)=f(x)$, This implies that we want

$$
F_e(x)-f(x)=a_{0}+a_{1}\cos(x)+a_{2}\cos(2x)+a_{1}\cos(3x)+\cdots
$$

If this is true, then we also want 

$$
\int_{-\pi}^{\pi}f(x)=\int_{-\pi}^{\pi}a_{0}+a_{1}\cos(x)+a_{2}\cos(2x)+a_{3}\cos(3x)+\cdots dx
$$

1. Use the above equation to find $a_{0}$ in terms of $\int_{-\pi}^{\pi}f(x)$

    $$
    \begin{align}
    \int_{-\pi}^{\pi}f(x)&=\int_{-\pi}^{\pi}a_{0}+a_{1}\cos(x)+a_{2}\cos(2x)+\cdots dx\\
    &= 2\pi a_{0} + \sum_{n=1}^{\infty}a_{n}\int_{-\pi}^{\pi}\cos(nx) dx\\
    \end{align}
    $$

    The area under the curve of $\cos(nx)$ (given $n$ is an integer where $n \neq 0$) over the interval $[-\pi,\pi]$ is zero, since $n$ describes the number of complete waves within a period of $2\pi$. In other words:

    $$
    \begin{align}
    \int_{-\pi}^{\pi}\cos(nx) dx = 0
    \end{align}
    $$

    $$
    \begin{align}
    \int_{-\pi}^{\pi}f(x) &= 2\pi a_{0} + \sum_{n=1}^{\infty}a_{n}\int_{-\pi}^{\pi}\cos(nx) dx\\
    &= 2\pi a_{0}\\\\
    a_0 &= \frac{1}{2\pi}\int_{-\pi}^{\pi}f(x)dx
    \end{align}
    $$

2. Simplify $\cos(nx+mx)+\cos(nx-mx)$ using trigonometric identities. Use those simplifications to evaluate $\int_{-\pi}^{\pi}\cos(nx)\cos(mx)dx$ when $m\ne n$. (Assume that $m$, $n$ are integers).

    $$
    \begin{align}
    &\cos(nx+mx)+\cos(nx-mx)\\
    &= [\cos(nx)\cos(mx)-\sin(nx)\sin(mx)]+[\cos(nx)\cos(mx)+\sin(nx)\sin(mx)]\\
    &= 2\cos(nx)\cos(mx)\\
    \end{align}
    $$

    $$
    \begin{align}
    \int_{-\pi}^{\pi}\cos(nx)\cos(mx)dx &= \int_{0}^{\pi}2\cos(nx)\cos(mx)dx\\
    &= \int_{0}^{\pi}\cos(nx+mx)+\cos(nx-mx)dx\\
    &= \int_{0}^{\pi}\cos(nx+mx)dx+\int_{0}^{\pi}\cos(nx-mx)dx\\
    &= 0
    \end{align}
    $$

    The area under the curve of $\cos(nx)$ (given $n$ is any integer where $n \neq 0$) over the interval $[0,\pi]$ is zero, since $n$ describes half the number of complete waves within a period of $\pi$. (Similar to #1)

3. Now consider the previous question, but now let $m=n$ Evaluate $\int_{-\pi}^{\pi}\cos(nx)\cos(mx)dx$ (Hint: It will be useful to simplify the integrand before integrating)

    $$
    \begin{align}
    \int_{-\pi}^{\pi}\cos(nx)\cos(mx)dx &= \int_{-\pi}^{\pi}\cos(nx)\cos(nx)dx\\
    &= \int_{0}^{\pi}2\cos(nx)\cos(nx)dx\\
    &= 2\int_{0}^{\pi}\cos^{2}(nx)dx\\
    &= 2\int_{0}^{\pi}\frac{1+\cos(2nx)}{2}dx\\
    &= \int_{0}^{\pi}1+\cos(2nx)dx\\
    &= \pi
    \end{align}
    $$

4. Use the result from the previous questions to find the value of $a_{1}$ in terms of $\int_{-\pi}^{\pi}\cos(x)f(x)dx$, knowing that $\int_{-\pi}^{\pi}\cos(x)f(x)dx=\int_{-\pi}^{\pi}a_{0}\cos{x}+a_{1}\cos^{2}{x}+a_{2}\cos{x}\cos{2x}+\cdots dx$

    $$
    \begin{align}
    \int_{-\pi}^{\pi}\cos(x)f(x)dx&=\int_{-\pi}^{\pi}a_{0}\cos{x}+a_{1}\cos^{2}{x}+a_{2}\cos{x}\cos{2x}+\cdots dx\\
    &= \int_{-\pi}^{\pi}a_{0}\cos{x}+a_{1}\cos^{2}{x} dx\\
    &= \frac{a_{1}}{2}\int_{-\pi}^{\pi}1+\cos(2x)dx\\
    &= a_{1}\pi\\\\
    a_{1}&=\frac{1}{\pi}\int_{-\pi}^{\pi}\cos(x)f(x)dx
    \end{align}
    $$

5. Now use a similar procedure to the previous question to determine $a_{2}$ in terms of $\int_{-\pi}^{\pi}\cos{2x}f(x)dx.$

    $$
    \begin{align}
    \int_{-\pi}^{\pi}\cos(2x)f(x)dx&=\int_{-\pi}^{\pi}a_{0}\cos{2x}+a_{1}\cos{x}\cos{2x}+a_{2}\cos^2{2x}+\cdots dx\\
    &= \int_{-\pi}^{\pi}a_{2}\cos^2{2x}dx\\
    &= \frac{a_{2}}{2}\int_{-\pi}^{\pi}1+\cos(4x)dx\\
    &= a_{2}\pi\\\\
    a_{2}&=\frac{1}{\pi}\int_{-\pi}^{\pi}\cos(2x)f(x)dx
    \end{align}
    $$

6. Repeat to find $a_{3}$ in terms of $\int_{-\pi}^{\pi}\cos{3x}f(x)$.

    $$
    \begin{align}
    \int_{-\pi}^{\pi}\cos(3x)f(x)dx&=\int_{-\pi}^{\pi}a_{0}\cos{3x}+a_1\cos{x}\cos{3x}+\cdots+a_{3}\cos^2{3x}+\cdots dx\\
    &= \int_{-\pi}^{\pi}a_{3}\cos^2{3x}dx\\
    &= \frac{a_{3}}{2}\int_{-\pi}^{\pi}1+\cos(6x)dx\\
    &= a_{3}\pi\\\\
    a_{3}&=\frac{1}{\pi}\int_{-\pi}^{\pi}\cos(3x)f(x)dx
    \end{align}
    $$

7. Now generalize to find $a_{n}$ in terms of $\int_{-\pi}^{\pi}\cos{nx}f(x)dx$. (For $n\ge 1$)

    $$
    \begin{align}
    \int_{-\pi}^{\pi}\cos(nx)f(x)dx&=\int_{-\pi}^{\pi}\cdots + a_{n-1}\cos{x}\cos{nx}+a_{n}\cos^2{nx}+\cdots dx\\
    &= \int_{-\pi}^{\pi}a_{n}\cos^2{nx}dx\\
    &= \frac{a_{n}}{2}\int_{-\pi}^{\pi}1+\cos(2nx)dx\\
    &= a_{n}\pi\\\\
    a_{n}&=\frac{1}{\pi}\int_{-\pi}^{\pi}\cos(nx)f(x)dx
    \end{align}
    $$

8. Now let $f(x)=e^{-x^{2}}$, the interval $[-\pi,\pi]$. Use a calculator to determine the coefficients $a_{0}$, $a_{1}$, $a_{2}$ , $a_{3}$, $a_{4}$ and $a_{5}$ Graph $e^{-x^{x}}$ on the interval $[-\pi,\pi]$ and compare it to the graph of your series, $F_{e}(x)=a_{0}+a_{1}cos(x)+a_{2}cos(2x)+\cdot\cdot\cdot+a_{5}cos(5x)$ on the same interval.

$$
\begin{aligned}
a_0 &= \frac{1}{2\pi}\int_{-\pi}^{\pi}e^{-x^{2}}dx &\approx 0.28209\\
a_1 &= \frac{1}{\pi}\int_{-\pi}^{\pi}e^{-x^{2}}\cos(x)dx &\approx 0.43939\\
a_2 &= \frac{1}{\pi}\int_{-\pi}^{\pi}e^{-x^{2}}\cos(2x)dx &\approx 0.20754\\
a_3 &= \frac{1}{\pi}\int_{-\pi}^{\pi}e^{-x^{2}}\cos(3x)dx &\approx 0.05946\\
a_4 &= \frac{1}{\pi}\int_{-\pi}^{\pi}e^{-x^{2}}\cos(4x)dx &\approx 0.01032\\
a_5 &= \frac{1}{\pi}\int_{-\pi}^{\pi}e^{-x^{2}}\cos(5x)dx &\approx 0.00109\\\\
\end{aligned}
$$

$$
F_e(x) = 0.28209 + 0.43939\cos(x) + 0.20754\cos(2x) + \cdots + 0.00109\cos(5x)
$$

<iframe src="https://www.desmos.com/calculator/ixkivqtoux?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

On the next take-home quiz, you will be thinking about odd function Fourier series, and then generalizing to all functions!