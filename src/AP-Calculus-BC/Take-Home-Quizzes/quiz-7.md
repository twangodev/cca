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

<iframe src="https://www.desmos.com/calculator/g9x9aptg8n?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

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

2. Simplify $\cos(nx+mx)+\cos(nx-mx)$ using trigonometric identities. Use those en simplifications to evaluate $\int_{-\pi}^{\pi}cos(nx)cos(mx)dx$ when $m\ne n$. (Assume that $m$, $n$ are integers).

3. Now consider the previous question, but now let $m=n$ Evaluate $\int_{-\pi}^{\pi}\cos(nx)\cos(mx)dx$ (Hint: It will be useful to simplify the integrand before integrating)

4. Use the result from the previous questions to find the value of $a_{1}$ in terms of $\int_{-\pi}^{\pi}\cos{x}f(x)dx$, knowing that $\int_{-\pi}^{\pi}\cos{x}f(x)dx=\int_{-\pi}^{\pi}a_{0}\cos{x}+a_{1}\cos^{2}{x}+a_{2}\cos{x}\cos{2x}+a_{3}\cos{x}\cos{3x}+\cdots dx$

5. Now use a similar procedure to the previous question to determine $a_{2}$ in terms of $\int_{-\pi}^{\pi}\cos{2x}f(x)dx.$

6. Repeat to find $a_{3}$ in terms of $\int_{-\pi}^{\pi}\cos{3x}f(x)$.

7. Now generalize to find $a_{n}$ in terms of $\int_{-\pi}^{\pi}\cos{nx}f(x)dx$. (For $n\ge 1$)

8. Now let $f(x)=e^{-x^{2}}$, the interval $[-\pi,\pi]$. Use a calculator to determine the coefficients $a_{0}$, $a_{1}$, $a_{2}$ , $a_{3}$, $a_{4}$ and $a_{5}$ Graph $e^{-x^{x}}$ on the interval $[-\pi,\pi]$ and compare it to the graph of your series, $F_{e}(x)=a_{0}+a_{1}cos(x)+a_{2}cos(2x)+\cdot\cdot\cdot+a_{5}cos(5x)$ on the same interval.

On the next take-home quiz, you will be thinking about odd function Fourier series, and then generalizing to all functions!