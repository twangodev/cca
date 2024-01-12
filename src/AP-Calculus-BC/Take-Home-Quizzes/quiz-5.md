# Take Home Quiz 5: Supplemental AP Calculus BC Final Exam

1. Let $f$ be the function that has derivatives of all orders (i.e. can be differentiated any number of times). Let $3-6(x-1)^2 + 5(x-3)^3 - 2(x-1)^4$ be the fourth-degree Taylor polynomial for $f$ about $x=1$. Does $f$ have a local minimum, local maximum, or neither at $x=1$? Explain how you know.

    From the equation, the following can be determined with the Taylor Series:

    $$
    \frac{f(1)}{0!} = 3, \frac{f'(1)}{1!} = 0, \frac{f''(1)}{2!} = -6 
    $$

    The function has a critical point at $x=1$ since $f'(1) = 0$. Since $f''(1) = -12 < 0$, the function has a local maximum at $x=1$.

2. Evaluate the following integrals:
    1. $\int_{-1}^1 \frac{1}{x^2} dx$
   
        $$ 
        \begin{aligned}
        &= \int_{-1}^0 \frac{1}{x^2} dx + \int_{0}^1 \frac{1}{x^2} dx\\
        &= -\frac{1}{x} \Biggr|_{-1}^{0} + \frac{1}{x} \Biggr|_{0}^{1}\\
        &= \text{Divergent}
        \end{aligned}
        $$

    2. $\int_{-\infty}^{\infty} \frac{1}{1+x^2} dx$

        $$
        \begin{aligned}
        &= \tan^{-1}(x) \Biggr|_{-\infty}^{\infty}\\
        &= \lim_{x \to \infty} \tan^{-1}(x) - \lim_{x \to -\infty} \tan^{-1}(x)\\
        &= \frac{\pi}{2} - \frac{-\pi}{2}\\
        &= \pi
        \end{aligned}
        $$

    3. $\int_{-3}^3 \frac{x}{1+|x|} dx$

        $$
        \begin{aligned}
        f(x) &= \frac{x}{1+|x|}\\
        f(-x) &= \frac{-x}{1+|-x|}\\
        &= \frac{-x}{1+|x|}\\
        f(x) &= f(-x) \text{ (Odd function)} \\
        \therefore \int_{-3}^3 \frac{x}{1+|x|} dx &= 0
        \end{aligned}
        $$

    4. $\int \frac{dx}{e^x \sqrt{4-e^{-2x}}}$

        $$
        \begin{aligned}
        u = e^{-x}&, du = -e^{-x} dx\\
        \int \frac{dx}{e^x \sqrt{4-e^{-2x}}}dx &= \int \frac{-du}{\sqrt{4-u^2}}\\
        &= -\sin^{-1}(\frac{u}{2}) + C\\
        &= -\sin^{-1}(\frac{e^{-x}}{2}) + C
        \end{aligned}
        $$

3. Find the sum of the following series:
    1. $2 - \sqrt{2} + 1 - \frac{\sqrt{2}}{2} + \frac{1}{2} - \dots$

        $$
        \begin{aligned}
        &= \sum_{n=0}^{\infty} 2(\frac{1}{2})^n - \sum_{n=0}^{\infty} \sqrt{2}(\frac{1}{2})^n\\
        &= \frac{2}{1-\frac{1}{2}} - \frac{\sqrt{2}}{1-\frac{1}{2}}\\
        &= 4 - 2\sqrt{2}
        \end{aligned}
        $$

    2. $\sum_{n=0}^{\infty} \frac{2^{n-1}}{n!}$

        $$
        \begin{aligned}
        &= \sum_{n=0}^{\infty} \frac{2^n}{2n!}\\
        &= \frac{1}{2} \sum_{n=0}^{\infty} \frac{2^n}{n!}\\
        \end{aligned}
        $$
        
        Using the Maclaurin Series for $e^x$:       

        $$
        \begin{aligned}
        e^x &= \sum_{n=0}^{\infty} \frac{x^n}{n!}\\
        \frac{1}{2} \sum_{n=0}^{\infty} \frac{2^n}{n!} &= \frac{e^2}{2}
        \end{aligned}
        $$

    3. $3 \sum_{n=0}^{\infty} \frac{(-1)^n (\sqrt{3})^{2n+1}}{2n+1}$
    
        Given the Maclaurin Series for $\tan^-1(x)$:
   
        $$
        \begin{aligned}
        \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n+1}}{2n+1} &= \tan^{-1}(x)\\
        \sum_{n=0}^{\infty} \frac{(-1)^n (\sqrt{3})^{2n+1}}{2n+1} &= \tan^{-1}(\sqrt{3})
        \end{aligned}
        $$
   
    4. $\sum_{k=1}^{\infty} \ln(\frac{k}{k+1})$

        $$
        \begin{aligned}
        &= \sum_{k=1}^{\infty} \ln(k) - \ln(k+1)\\
        &= \ln(1) - \ln(2) + \ln(2) - \ln(3) + \ln(3) - \ln(4) + \dots\\
        &= 0 \text{ (Telescoping series)}
        \end{aligned}
        $$

    5. $\sum_{n=1}^{\infty} \frac{\sqrt{n+1}-\sqrt{n}}{\sqrt{n(n+1)}}$

        $$
        \begin{aligned}
        &= \sum_{n=1}^{\infty} \frac{\sqrt{n+1}}{\sqrt{n(n+1)}} - \frac{\sqrt{n}}{\sqrt{n(n+1)}}\\
        &= 1 \text{ (Telescoping series)}
        \end{aligned}
        $$

4. For what values of $r$ is the integral $\int_{0}^{\infty} \frac{1}{x^r} dx$ convergent?

    Between $0$ and $1$, the integral is convergent for $r > 1$. For $r \leq 1$, the integral is divergent.

    Between $1$ and $\infty$, the integral is convergent for $r < 1$. For $r \geq 1$, the integral is divergent.

    Therefore, no combination of $r$ values will make the integral convergent. One section of the integral will always be divergent, so the entire integral is divergent since the integral $\int_{0}^{\infty} \frac{1}{x^r} dx$ is made up from $\int_{0}^{1} \frac{1}{x^r} dx + \int_{1}^{\infty} \frac{1}{x^r} dx$.

5. The sum of an infinite geometric series with common ratio $r$ is 15, and the sum of the squares of the terms of this series 45. What is the first term of the series?

    $$
    \begin{aligned}
    \begin{cases}
    \frac{a}{1-r} = 15\\
    \frac{a^2}{1-r^2} = 45
    \end{cases}\\
    a &= 15(1-r)\\
    45 &= \frac{(15(1-r))^2}{1-r^2}\\
    45(1-r^2) &= 15^2(1-r)^2\\
    270r^2 - 450r + 180 &= 0\\
    3r^2 - 5r + 2 &= 0\\
    (3r - 2)(r - 1) &= 0\\
    r &= \frac{2}{3}, 1 \text{ (Cannot have } r = 1 \text{)}\\
    a &= 15(1-\frac{2}{3})\\
    &= 5
    \end{aligned}
    $$

6. Determine if the following series are absolutely convergent, conditionally convergent, or divergent.
    1. $\sum_{n=2}^{\infty} \frac{(-1)^n}{n(\ln{n})^3}$

        Using the integral test:
   
        $$
        \begin{aligned}
        \int_{2}^{\infty} \frac{1}{x(\ln{x})^3} dx &= \frac{1}{2\ln(2)^2} \text{ (Convergent)}\\
        \end{aligned} 
        $$

        Passes the alternating series test, therefore it is absolutely convergent.

    2. $\sum_{n=1}^{\infty} \frac{(n!)^2}{(2n)!}$
   
        Using the ratio test:
 
        $$
        \begin{aligned}
        \lim_{n \to \infty} \frac{(n+1)!^2}{(2n+2)!} \cdot \frac{(2n)!}{(n!)^2} &= \lim_{n \to \infty} \frac{(n+1)^2}{(2n+2)(2n+1)}\\
        &= \frac{1}{4} \text{ (Absolutely Convergent)}\\
        \end{aligned}
        $$
   
    3. $\sum_{n=1}^{\infty} a_n \text{ where } a_1=2, a_{n+1} = \frac{2n+1}{5n-4}$
   
        Using the ratio test:
 
        $$
        \begin{aligned}
        \lim_{n \to \infty} \frac{a_{n+1}}{a_n} &= \lim_{n \to \infty} \frac{2n+1}{5n-4} \cdot \frac{5n-9}{2n-1}\\
        &= \frac{2}{5} \text{ (Absolutely Convergent)}\\
        \end{aligned}
        $$

7. Let $f(x) = 1 + \frac{x}{2} + \frac{x^2}{4} + \frac{x^3}{8} + \dots = \sum_{n=0}^{\infty} \frac{x^n}{2^n}$ for $-1 \leq x \leq 1$. Determine $\sqrt{e^{\int_{0}^{1} f(x) dx}}$.

    $$
    \begin{aligned}
    \int_{0}^{1} f(x) dx &= \sum_{n=0}^{\infty} \frac{x^n}{2^n} dx\\
    &= \sum_{n=0}^{\infty} (\frac{x}{2})^n \\
    &= \frac{2}{2-x}\\
    &\int_{0}^{1} \frac{2}{2-x}\\
    u = 2-x&, du = -dx\\
    &= \int_{1}^{2} \frac{-2}{u} du\\
    &= -2\ln(u) \Biggr|_{1}^{2}\\
    &= -2\ln(2) + 2\ln(1)\\
    &= -2\ln(2)\\
    \sqrt{e^{2\ln2}} &= e^{\ln2}\\
    &= 2
    \end{aligned}
    $$

8. Consider the following series

    $$\frac{1}{2} - \frac{1}{3} + \frac{1}{2^2} - \frac{1}{3^2} + \frac{1}{2^3} - \frac{1}{3^3} + \dots$$

    1. Explain why it is not possible to use the alternating series test on this series.

        The series is not monotonically decreasing since the terms alternate between $\frac{1}{2^n}$ and $\frac{1}{3^n}$.

    2. This series actually does converge! Find the sum of the series. (Hint: Split the series up)

        $$
        \begin{aligned}
        &= \sum_{n=1}^{\infty} \frac{1}{2^n} - \sum_{n=1}^{\infty} \frac{1}{3^n}\\
        &= \frac{\frac{1}{2}}{1-\frac{1}{2}} - \frac{\frac{1}{3}}{1-\frac{1}{3}}\\
        &= 1 - \frac{1}{2}\\
        &= \frac{1}{2}
        \end{aligned}
        $$

9. Find the values of $p$ which make the following series converge:
    1. $\sum_{n=1}^{\infty} (-1)^n \frac{1}{n + p}$
   
        For any value of $p$, the series will converge since it is an alternating series.

    2. $\sum_{n=1}^{\infty} n(1+n^2)^p$

        The largest dominating term is $n^{2p+1}$, therefore the series will converge for $2p + 1 < -1$. Therefore, the series will converge for $p < -1$.

    3. $\sum_{n=1}^{\infty} \frac{(n!)^2}{(pn)!}$

        The ratio test can be used to determine the values of $p$ that make the series converge:

        $$
        \begin{aligned}
        \lim_{n \to \infty} \frac{(n+1)!^2}{(p(n+1))!} \cdot \frac{(pn)!}{(n!)^2} &= \lim_{n \to \infty} \frac{(n+1)^2}{(pn+1)(pn+2)(pn+3)\dots(pn+p)}\\
        &= \frac{1}{p^p} \\
        p &\geq 2\\
        \end{aligned}
        $$

10. If $f(x) = \sin(x^3)$, then find $f^{(15)}(0)$. (Hint: This means 15th derivative) (Hint 2: Don't try to take 15 derivatives since it would get unbearably messy)

    With the Maclaurin Series: 

    $$
    \begin{aligned}
    \sin(x) &= \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n+1}}{(2n+1)!}\\
    &= x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + \cdots\\
    \sin(x^3) &= x^3 - \frac{x^9}{3!} + \frac{x^{15}}{5!} - \frac{x^{21}}{7!} + \cdots\\
    \end{aligned}
    $$

    By definition of the terms of the Maclaurin Series:

    $$
    \begin{aligned}
    \frac{f^{(15)}(0)}{15!}x^15 &= \frac{x^{15}}{5!}\\
    \frac{f^{(15)}(0)}{15!} &= \frac{1}{5!}\\
    f^{(15)}(0) &= \frac{15!}{5!}\\
    &= 10,897,286,400
    \end{aligned}
    $$

11. Find $F'(0)$ if $F(x) = \begin{cases} \frac{g(x)\sin^2x}{x} & x \neq 0 \\ 0 & x = 0 \end{cases}$ (Hint: Your answer should be in terms of $g$)

    $$
    \begin{aligned}
    F'(0) &= \lim_{x \to 0} \frac{F(x) - F(0)}{x - 0}\\
    &= \lim_{x \to 0} \frac{\frac{g(x)\sin^2x}{x} - 0}{x}\\
    &= \lim_{x \to 0} \frac{g(x)\sin^2x}{x^2} \Rightarrow \frac{0}{0}\\
    &= \lim_{x \to 0} \frac{2g(x)\sin x\cos x + \sin^2xg'(x)}{2x} \text{ LH} \Rightarrow \frac{0}{0}\\
    &= \lim_{x \to 0} \frac{2g(x)(\cos^2x - \sin^2x) + 4g'(x)\sin x\cos x + g''(x)\sin^2x}{2} \text{ LH}\\
    &= \frac{2g(0)(1 - 0) + 4g'(0)(0)(1) + g''(0)(0)}{2}\\
    &= \frac{2g(0)}{2}\\
    &= g(0)
    \end{aligned}
    $$
