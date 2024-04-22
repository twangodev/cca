# Conditional Convergence

One of the topics we've discussed this school year was the concept of absolute vs. conditional convergence. But what does conditionally convergent really mean? This example will give a glimpse into what that is (because I don't fully understand what conditional convergence truly is... :frowning:)

1. Write the first eight non-zero terms and the general term for the function $f(x) = \frac{1}{1-x}$ and determine its interval of convergence.

    **First Eight Non-Zero Terms and General Term:**

    $$
    \begin{align}
    \frac{1}{1-x} &= 1 + x + x^2 + x^3 + x^4 + x^5 + x^6 + x^7 + \cdots \\
    &= \sum_{n=0}^{\infty} x^n
    \end{align}
    $$

    **Interval of Convergence:**

    $$
    \begin{align}
    \lim_{n \to \infty} \left| \frac{x_{n+1}}{x_n} \right| &= x < 1\\\\
    x = -1: \text{ Divergent} \\ 
    x = 1: \text{ Divergent} \\
    \therefore (-1, 1)
    \end{align}
    $$

2. Find the first eight non-zero terms and the general term for the function $g(x) = \ln(1+x)$ based on the previous question. Determine the interval of convergence. Is the interval of convergence different from the previous question?

    **First Eight Non-Zero Terms and General Term:**

    $$
    \begin{align}
    \int \frac{1}{1+x} dx &= \int \sum_{n=0}^{\infty} x^n dx \\
    &= \ln(1+x) + C \\\\
    \ln(1+x) &= x - \frac{x^2}{2} + \frac{x^3}{3} - \frac{x^4}{4} + \frac{x^5}{5} - \frac{x^6}{6} + \frac{x^7}{7} - \cdots \\
    &= \sum_{n=1}^{\infty} (-1)^{n+1} \frac{x^n}{n}
    \end{align}
    $$

    **Interval of Convergence:**

    $$
    \begin{align}
    \lim_{n \to \infty} \left| \frac{\frac{x^{n+1}}{n+1}}{\frac{x^n}{n}} \right| = \lim_{n \to \infty} \left| \frac{nx^{n+1}}{x^n (n+1)} \right| &< 1 \\
    \lim_{n \to \infty} \left| \frac{xn}{n+1} \right| &< 1 \\
    x \lim_{n \to \infty} \left| \frac{n}{n+1} \right| &< 1 \\
    x &< 1 \\\\
    x = -1: \text{ Divergent} \\
    x = 1: \text{ Convergent} \\\\
    \therefore (-1, 1]
    \end{align}
    $$

3. Based on your series from #2, determine what $\ln(2)$ is equal to in series form. (Again, write the first eight non-zero terms and the general term.) The series for $\ln(2)$ should look familiar. What do we call that series?

    **Substitute $x=1$:**

    $$
    \begin{align}
    \ln(x+1) &= \sum_{n=1}^{\infty} (-1)^{n+1} \frac{x^n}{n} \\\\
    \ln(2) &= 1 - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \frac{1}{5} - \frac{1}{6} + \frac{1}{7} - \cdots \\
    &= \sum_{n=1}^{\infty} (-1)^{n+1} \frac{1}{n} \text{ (Alternating Harmonic Series)}
    \end{align}
    $$

4. Now consider manipulation of the series for $\ln(2)$ from #3. For **only** the positive terms (which have the form of $\frac{1}{n}$), rewrite them in the manner of $\frac{2}{n} - \frac{1}{n}$. Leave the negative terms alone. This will still be equal to $\ln(2)$ of course. (You do **not** need to simplify.) 

    $$
    \begin{align}
    \ln(2) &= \frac{2}{1} - \frac{1}{2} + \frac{2}{3} - \frac{1}{4} + \frac{2}{5} - \frac{1}{6} + \frac{2}{7} - \cdots \\
    &= \ln(2) = \left(2 - 1\right) - \frac{1}{2} + \left(\frac{2}{3} - \frac{1}{3}\right) - \frac{1}{4} + \left(\frac{2}{5} - \frac{1}{5}\right) - \frac{1}{6} + \cdots
    \end{align}
    $$

5. Now multiply both sides of the equation by $\frac{1}{2}$. The left is, obviously, $\frac{\ln(2)}{2}$. For the right side, distribute into the parenthesis first, then remove the parenthesis, **without** simplifying or reordering anything (but reduce the fractions.) What do you notice about this new series, compared to the one for $\ln(2)$? What's surprising about this result?

    $$
    \begin{align}
    \frac{\ln(2)}{2} &= \frac{1}{2}(2 - 1) - \frac{1}{2} \cdot \frac{1}{2} + \frac{1}{2}\left(\frac{2}{3} - \frac{1}{3}\right) - \frac{1}{2} \cdot \frac{1}{4} + \frac{1}{2}\left(\frac{2}{5} - \frac{1}{5}\right) + \cdots\\
    &= \left(\frac{2}{2} - \frac{1}{2}\right) - \frac{1}{4} + \left(\frac{2}{6} - \frac{1}{6}\right) - \frac{1}{8} + \left(\frac{2}{10} - \frac{1}{10}\right) - \frac{1}{12} + \cdots\\
    &= \left(1 - \frac{1}{2}\right) - \frac{1}{4} + \left(\frac{1}{3} - \frac{1}{6}\right) - \frac{1}{8} + \left(\frac{1}{5} - \frac{1}{10}\right) - \frac{1}{12} + \cdots\\
    &= 1 - \frac{1}{2} - \frac{1}{4} + \frac{1}{3} - \frac{1}{6} - \frac{1}{8} + \frac{1}{5} - \frac{1}{10} - \frac{1}{12} + \cdots\\
    \end{align}
    $$

    What is suprising is that $\frac{\ln(2)}{2}$ seems to have the same terms as $\ln(2)$ - just rearranged. But it's technically half of $\ln(2)$.

6. Now consider another manipulation. Take the series for $\ln(2)$ from #3, multiply both sides by $\frac{1}{2}$, and add this new series to $\ln(2)$. On the left side, you get $\frac{3\ln(2)}{2}$. On the right, combine terms with the same denominators, with the denominators in increasing order. Simplify the terms with the same denominator, remove zeroes, but **don't** reorder anything. What do you get on the right side? (It should look like a variation of something familiar.)

    $$
    \begin{align}
    \ln(2) &= \frac{1}{1} - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \frac{1}{5} - \frac{1}{6} + \frac{1}{7} - \cdots \\
    \frac{\ln(2)}{2} &= \frac{1}{2} - \frac{1}{4} + \frac{1}{6} - \frac{1}{8} + \frac{1}{10} - \frac{1}{12} + \cdots \\\\
    \ln(2) + \frac{\ln(2)}{2} &= \frac{3\ln(2)}{2} = 1 + \left(-\frac{1}{2} + \frac{1}{2}\right) + \frac{1}{3} + \left(-\frac{1}{4} - \frac{1}{4}\right) + \frac{1}{5} + \cdots \\
    &= 1 + \frac{1}{3} - \frac{1}{2} + \frac{1}{5} - \frac{1}{4} + \frac{1}{7} + \cdots \\\\
    &\text{ (Alternating Harmonic Series)}
    \end{align}
    $$

7. Look at the series for $\ln(2)$ and consider the positive terms. What are the first four non-zero terms and general term for these positive terms? Do the same for the negative terms. Do either of these individual series converge? (This should be a pseudo-surprising result :smile:)

    **Positive Terms:**

    $$
    \begin{align}
    1 + \frac{1}{3} + \frac{1}{5} + \frac{1}{7} + \cdots= \sum_{n=0}^{\infty} \frac{1}{2n+1}\\
    \left(\text{Divergent via Direct Comparison with } \frac{1}{n}\right)
    \end{align}
    $$

    **Negative Terms:**

    $$
    \begin{align}
    - \frac{1}{2} - \frac{1}{4} - \frac{1}{6} - \frac{1}{8} - \cdots= \sum_{n=0}^{\infty} \frac{1}{2n}\\
    \left(\text{Divergent via Direct Comparison with } \frac{1}{n}\right)
    \end{align}
    $$

    What's interesting is that since both the positive and negative terms are divergent. However, the sum of the positive and negative terms make $\ln(2)$ convergent. What makes it conditionally convergent is the fact the alternation of the positive and negative terms "cancels out" the divergence of each of the individual series. When you look at whether its absolute convergence though, you ignore the alternation, and thus the series is divergent (equivalent to a harmonic series).