# Cheatsheet

## Limits

### Trigonometric Limits
$$
\begin{align}
\lim_{x \to 0} \frac{\sin ax}{ax} &= 1 \\\\
\lim_{x \to 0} \frac{1 - \cos ax}{ax} &= 0 \\\\
\end{align}
$$

### L'Hopital's Rule
When evaluating a limit to an indeterminate form, you can use L'Hopital's Rule to evaluate the limit:

$$
\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)} \quad \text{or} \quad \lim_{x \to \infty} \frac{f(x)}{g(x)} = \lim_{x \to \infty} \frac{f'(x)}{g'(x)}
$$

### Intermediate Value Theorem

If $f$ is continuous on $[a, b]$ and $N$ is between $f(a)$ and $f(b)$, then there exists a number $c$ in $[a, b]$ such that $f(c) = N$.

### Mean Value Theorem

If $f$ is continuous on $[a, b]$ and differentiable on $(a, b)$, then there exists a number $c$ in $(a, b)$ such that:

$$ f'(c) = \frac{f(b) - f(a)}{b - a} $$

## Derivatives

### Trigonometric Derivatives

$$
\begin{align}
\frac{d}{dx} \sin x &= \cos x \\\\
\frac{d}{dx} \cos x &= -\sin x \\\\
\frac{d}{dx} \tan x &= \sec^2 x \\\\
\frac{d}{dx} \sec x &= \sec x \tan x \\\\
\frac{d}{dx} \csc x &= -\csc x \cot x \\\\
\frac{d}{dx} \cot x &= -\csc^2 x \\\\
\end{align}
$$

### Inverse Trigonometric Derivatives

$$
\begin{align}
\frac{d}{dx} \sin^{-1} x &= \frac{1}{\sqrt{1 - x^2}} \\\\
\frac{d}{dx} \cos^{-1} x &= -\frac{1}{\sqrt{1 - x^2}} \\\\
\frac{d}{dx} \tan^{-1} x &= \frac{1}{1 + x^2} \\\\
\frac{d}{dx} \sec^{-1} x &= \frac{1}{|x|\sqrt{x^2 - 1}} \\\\
\frac{d}{dx} \csc^{-1} x &= -\frac{1}{|x|\sqrt{x^2 - 1}} \\\\
\frac{d}{dx} \cot^{-1} x &= -\frac{1}{1 + x^2} \\\\
\end{align}
$$

### Inverse Function

If $f$ is a one-to-one function, then the inverse function $f^{-1}$ has the derivative:

$$
\frac{d}{dx} f^{-1}(x) = \frac{1}{f'(f^{-1}(x))}
$$

## Integrals

### Fundamental Theorem of Calculus

If $f$ is continuous on $[a, b]$, then:

$$
\int_a^b f(x) \, dx = F(b) - F(a)
$$

where $F$ is an antiderivative of $f$.

### Average Value of a Function

The average value of a function $f$ on $[a, b]$ is:

$$
\frac{1}{b - a} \int_a^b f(x) \, dx
$$

## Parametric Equations

### Slope of a Parametric Curve

The slope of a parametric curve $x = f(t)$, $y = g(t)$ at a point $(x, y)$ is:

$$
\frac{dy}{dx} = \frac{g'(t)}{f'(t)} \quad \text{where} \quad \frac{dx}{dt} \neq 0
$$

### Velocity of a Parametric Curve

The velocity of a parametric curve $x = f(t)$, $y = g(t)$ at a point $(x, y)$ is:

$$
\sqrt{[f'(t)]^2 + [g'(t)]^2}
$$

### Velocity Vector of a Parametric Curve

The velocity vector of a parametric curve $x = f(t)$, $y = g(t)$ is:

$$
\langle f'(t), g'(t) \rangle
$$

### Arc Length of a Parametric Curve

The arc length of a parametric curve $x = f(t)$, $y = g(t)$ from $t = a$ to $t = b$ is:

$$
\int_a^b \sqrt{[f'(t)]^2 + [g'(t)]^2} \, dt
$$
