# Fourier Series (Part 2)

## Introduction and Derivation of Fourier Series

Previously, you looked at Fourier series and derived what an even Fourier series would look like for a function. Now we are going to determine what the Fourier series would be like for an odd function and a general function.

## Fourier Series for Odd Functions

Remember that an odd function is a function that has the property $f(-x)=-f(x)$. The odd Fourier series will have the form

$$F_{0}(x)=b_{1}\sin(x)+b_{2}\sin(2x)+b_{3}\sin(3x)+\cdots$$

Similar to before, we want:

$$\int_{-\pi}^{\pi}f(x)=\int_{-\pi}^{\pi}b_{1}\sin(x)+b_{2}\sin(2x)+b_{3}\sin(3x)+\cdots dx$$

1. Using the definition of an odd function and looking at $F_{0}(x)$, explain why there cannot be a constant term $b_{0}$

    $$
    \begin{align}
    F_{0}(x) &= b_0 + b_{1}\sin(x)+b_{2}\sin(2x)+b_{3}\sin(3x)+\cdots\\
    F_{0}(-x) &= b_0 + b_{1}\sin(-x)+b_{2}\sin(-2x)+b_{3}\sin(-3x)+\cdots\\
    &= b_0 - b_{1}\sin(x)-b_{2}\sin(2x)-b_{3}\sin(3x)-\cdots\\
    &= b_0 - F_{0}(x)\\\\
    \therefore b_0 &= 0 \text{ given that } F_{0}(x) = -F_{0}(-x) \quad \blacksquare
    \end{align}
    $$

2. Simplify $\cos(mx+nx)-\cos(mx-nx)$ and use that to simplify $\int_{-\pi}^{\pi}\sin(nx)\sin(mx) dx$ when $m \ne n$ and when $m=n$. (Assume that $m$, $n$ are integers).

    $$
    \begin{align}
    &\cos(mx+nx)-\cos(mx-nx)\\
    &= -2\sin\left(\frac{(mx+nx)+(mx-nx)}{2}\right)\sin\left(\frac{(mx+nx)-(mx-nx)}{2}\right)\\
    &= -2\sin(mx)\sin(nx)\\\\
    \end{align}
    $$

    When $n=m$:

    $$
    \begin{align}
    &\int_{-\pi}^{\pi}\sin^2(nx) dx\\
    &= \int_{-\pi}^{\pi}\frac{1-\cos(2nx)}{2} dx\\
    &= \frac{1}{2}\left[x\right]_{-\pi}^{\pi} - \frac{1}{2}\int_{-\pi}^{\pi}\cos(2nx) dx\\
    &= \frac{1}{2}\cdot 2\pi\ - \frac{1}{2}\left[\frac{\sin(2nx)}{2n}\right]_{-\pi}^{\pi}\\
    &= \pi - \frac{1}{2}\left[\frac{\sin(0)}{2n}-\frac{\sin(0)}{2n}\right]\\
    &= \pi
    \end{align}
    $$

    When $n \ne m$:

    $$
    \begin{align}
    &\int_{-\pi}^{\pi}\sin(nx)\sin(mx)dx\\
    &= \frac{1}{2}\int_{-\pi}^{\pi}[\cos((m-n)x) + \cos((m+n)x)]dx\\
    &= \frac{1}{2}\left[\frac{\sin((m-n)x)}{m-n} + \frac{\sin((m+n)x)}{m+n}\right]_{-\pi}^{\pi}\\
    &= \frac{1}{2}\left[\frac{\sin(0)}{m-n} + \frac{\sin(0)}{m+n} - \frac{\sin(0)}{m-n} - \frac{\sin(0)}{m+n}\right]\\
    &= 0
    \end{align}
    $$

3. Use the previous result to find $b_{1}$ in terms of $\int_{-\pi}^{\pi}\sin(x)f(x)dx$.

    $$
    \begin{align}
    \int_{-\pi}^{\pi}\sin(x)f(x)dx &= \int_{-\pi}^{\pi}b_{1}\sin^2(x) + b_{2}\sin(x)\sin(2x) + \cdots dx\\
    &= b_{1}\int_{-\pi}^{\pi}\sin^2(x)dx\\
    &= b_{1}\pi\\\\
    \therefore b_{1} &= \frac{1}{\pi}\int_{-\pi}^{\pi}\sin(x)f(x)dx \quad \blacksquare
    \end{align}
    $$

4. Do the same for $b_{2}$ and $b_{3}$ and generalize for $b_{k}$ over the interval $[-\pi,\pi]$

    $$
    \begin{align}
    \int_{-\pi}^{\pi}\sin(2x)f(x)dx &= \int_{-\pi}^{\pi}b_{1}\sin(x)\sin(2x) + b_{2}\sin^2(2x) + \cdots dx\\
    &= b_{2}\int_{-\pi}^{\pi}\sin^2(2x)dx\\
    &= b_{2}\pi\\\\
    \therefore b_{2} &= \frac{1}{\pi}\int_{-\pi}^{\pi}\sin(2x)f(x)dx \quad \blacksquare
    \end{align}
    $$

    $$
    \begin{align}
    \int_{-\pi}^{\pi}\sin(3x)f(x)dx &= \int_{-\pi}^{\pi} \cdots + b_{2}\sin(2x)\sin(3x) + b_{3}\sin^2(3x) + \cdots dx\\
    &= b_{3}\int_{-\pi}^{\pi}\sin^2(3x)dx\\
    &= b_{3}\pi\\\\
    \therefore b_{3} &= \frac{1}{\pi}\int_{-\pi}^{\pi}\sin(3x)f(x)dx \quad \blacksquare
    \end{align}
    $$

    $$
    \begin{align}
    \int_{-\pi}^{\pi}\sin(kx)f(x)dx &= \int_{-\pi}^{\pi} \cdots + b_{k-1}\sin((k-1)x)\sin(kx) + b_{k}\sin^2(kx) + \cdots dx\\
    &= b_{k}\int_{-\pi}^{\pi}\sin^2(kx)dx\\
    &= b_{k}\pi\\\\
    \therefore b_{k} &= \frac{1}{\pi}\int_{-\pi}^{\pi}\sin(kx)f(x)dx \quad \blacksquare
    \end{align}
    $$

5. Now let $f(x)=\sin^{3}x$. Find the coefficients for $b_{1}$, $b_{2}$, $...$, $b_{5}$ and graph both the Fourier series and the original function over the interval $[-\pi,\pi]$.

    $$
    \begin{aligned}
    b_1 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\sin(x)\sin^{3}x dx &= 0.75\\
    b_2 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\sin(2x)\sin^{3}x dx &= 0\\
    b_3 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\sin(3x)\sin^{3}x dx &= -0.25\\
    b_4 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\sin(4x)\sin^{3}x dx &= 0\\
    b_5 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\sin(5x)\sin^{3}x dx &= 0\\
    \end{aligned}
    $$

    <iframe src="https://www.desmos.com/calculator/u6cmpfjmnd?embed" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>


6. Show, using identities, that the Fourier series that you generated is EXACTLY the same as $f(x)$.

$$
\begin{align}
\sin(3x) &= 3\cos^2(x)\sin(x) - \sin^3(x)\\
&= 3(1-\sin^2(x))\sin(x) - \sin^3(x)\\
&= 3\sin(x) - 3\sin^3(x) - \sin^3(x)\\
&= 3\sin(x) - 4\sin^3(x)\\\\
\therefore \sin^3(x) &= \frac{3}{4}\sin(x) - \frac{1}{4}\sin(3x)\\
\end{align}
$$


## General Fourier Series

Now we are going to consider the Fourier series for a general function.

1. What is the value of $\int_{-\pi}^{\pi}\sin(nx)\cos(mx)dx$ for all values of $n=m$. and $n\ne m$? (Hint: Remember that one function is odd, one function is even. What kind of function must their product be? What does that mean about the integral?)

    For $n=m$:

    $$
    \begin{align}
    &\int_{-\pi}^{\pi}\sin(nx)\cos(nx)dx\\
    &= \frac{1}{2}\int_{-\pi}^{\pi}\sin(nx + nx) + \sin(nx - nx)dx\\
    &= \frac{1}{2}\int_{-\pi}^{\pi}\sin(2nx)dx\\
    &= 0
    \end{align}
    $$

    When $n \ne m$:

    $$
    \begin{align}
    &\int_{-\pi}^{\pi}\sin(nx)\cos(mx)dx\\
    &= \frac{1}{2}\int_{-\pi}^{\pi}[\sin(nx + mx) + \sin(nx - mx)]dx\\
    &= \frac{1}{2}\int_{-\pi}^{\pi}[\sin((n+m)x) + \sin((n-m)x)]dx\\
    &= 0
    \end{align}
    $$

2. Since we are doing general Fourier series, now we are considering the function

    $$
    F(x)=a_{0}+a_{1}\cos(x)+b_{1}\sin(x)+a_{2}\cos(2x)+b_{2}\sin(2x)+\cdots
    $$

    Use $\int_{-\pi}^{\pi}f(x)=\int_{-\pi}^{\pi}F(x)$ to find $a_0$. (Hint: This should look familiar)

    $$
    \begin{align}
    \int_{-\pi}^{\pi}f(x) &= \int_{-\pi}^{\pi}a_{0}+a_{1}\cos(x)+b_{1}\sin(x)+a_{2}\cos(2x)+b_{2}\sin(2x)+\cdots dx\\
    &= 2\pi a_{0} + \int_{-\pi}^{\pi}a_{1}\cos(x)+b_{1}\sin(x)+\cdots dx\\
    \end{align}
    $$

    The area under the curve of $\cos(nx)$ and $\sin(nx)$ (given $n$ is an integer where $n \neq 0$) over the interval $[-\pi,\pi]$ is zero, since $n$ describes the number of complete waves within a period of $2\pi$. In other words:

    $$
    \int_{-\pi}^{\pi}\cos(nx) dx = 0 \text{ and } \int_{-\pi}^{\pi}\sin(nx) dx = 0
    $$

    $$
    \begin{align}
    \int_{-\pi}^{\pi}f(x) &= 2\pi a_{0} + \int_{-\pi}^{\pi}a_{1}\cos(x)+b_{1}\sin(x)+\cdots dx\\
    &= 2\pi a_{0}\\\\
    \therefore a_0 &= \frac{1}{2\pi}\int_{-\pi}^{\pi}f(x)dx \quad \blacksquare
    \end{align}
    $$

3. So now think of finding $a_{1}$ by multiplying $f(x)$ and $F(x)$ by $\cos(x)$. What two integrals will be set equal? Use these integrals to find $a_{1}$ in terms of $\int_{-\pi}^{\pi}f(x)$. (Hint: This should look familiar)

    $$
    \begin{align}
    \int_{-\pi}^{\pi}f(x)\cos(x) &= \int_{-\pi}^{\pi}a_{0}\cos(x)+a_{1}\cos^2(x)+b_{1}\sin(x)\cos(x)+\cdots dx\\
    &= a_{1}\int_{-\pi}^{\pi}\cos^2(x)dx\\
    &= a_{1}\pi\\\\
    \therefore a_{1} &= \frac{1}{\pi}\int_{-\pi}^{\pi}f(x)\cos(x)dx \quad \blacksquare
    \end{align}
    $$

4. Now multiply $f(x)$ and $F(x)$ by $\cos(nx)$ ($n=$ integer). Use this to find the pattern for $a_n$ (Hint: Again, should look familiar). (Hint 2: You should be using information from previous questions)

    $$
    \begin{align}
    \int_{-\pi}^{\pi}f(x)\cos(nx) &= \int_{-\pi}^{\pi}\cdots+a_{1}\cos(x)\cos(nx)+b_{1}\sin(x)\cos(nx)+\cdots dx\\
    &= a_{n}\int_{-\pi}^{\pi}\cos^2(nx)dx\\
    &= a_{n}\pi\\\\
    \therefore a_{n} &= \frac{1}{\pi}\int_{-\pi}^{\pi}f(x)\cos(nx)dx \quad \blacksquare
    \end{align}
    $$

5. Now do similar things as the previous question but multiplying by $\sin(mx)$ to find the pattern for $b_{n}$.

    $$
    \begin{align}
    \int_{-\pi}^{\pi}f(x)\sin(mx) &= \int_{-\pi}^{\pi}\cdots+a_{1}\cos(x)\sin(mx)+b_{1}\sin(x)\sin(mx)+\cdots dx\\
    &= b_{n}\int_{-\pi}^{\pi}\sin^2(mx)dx\\
    &= b_{n}\pi\\\\
    \therefore b_{n} &= \frac{1}{\pi}\int_{-\pi}^{\pi}f(x)\sin(mx)dx \quad \blacksquare
    \end{align}
    $$

6. Let $f(x)=\frac{1}{1+e^{x}}$. Find the coefficients $a_{0}$, $a_{1}$, $...$, $a_{5}$ and $b_{1}$, $b_{2}$, $...$, b_{5}.

    $$
    \begin{aligned}
    a_0 &= \frac{1}{2\pi}\int_{-\pi}^{\pi}\frac{1}{1+e^{x}}dx &= 0.5\\
    a_1 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\frac{1}{1+e^{x}}\cos(x)dx &= 0\\
    b_1 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\frac{1}{1+e^{x}}\sin(x)dx &= -.3913\\
    a_2 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\frac{1}{1+e^{x}}\cos(2x)dx &= 0\\
    b_2 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\frac{1}{1+e^{x}}\sin(2x)dx &= 0.1447\\
    a_3 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\frac{1}{1+e^{x}}\cos(3x)dx &= 0\\
    b_3 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\frac{1}{1+e^{x}}\sin(3x)dx &= -0.0982\\
    a_4 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\frac{1}{1+e^{x}}\cos(4x)dx &= 0\\
    b_4 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\frac{1}{1+e^{x}}\sin(4x)dx &= 0.0733\\
    a_5 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\frac{1}{1+e^{x}}\cos(5x)dx &= 0\\
    b_5 &= \frac{1}{\pi}\int_{-\pi}^{\pi}\frac{1}{1+e^{x}}\sin(5x)dx &= -0.0585\\
    \end{aligned}
    $$

7. Graph $f(x)$ and your 5th order Fourier approximation and compare on the interval $[-\pi,\pi]$

    <iframe src="https://www.desmos.com/calculator/ggmgipgd2b?embed" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>