# Taylor and MacLaurin Series

## Taylor Series

The Taylor Series is a representation of a function as an infinite sum of terms calculated from the values of its derivatives at a single point. 

If we have a function $f(x)$, we can write the Taylor Series for $f(x)$ as:

$$ 
f(x) = f(a) + f'(a)(x-a) + \frac{f''(a)(x-a)^2}{2!} + \cdots 
$$

This series expands a function into a series of terms, where each term is a derivative of the function evaluated at a certain point $a$, multiplied by $(x-a)$ raised to the power of the term's position in the series (starting from 0), and divided by the factorial of the term's position.

More simply written, the Taylor Series for $f(x)$ is:

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!}(x-a)^n
$$

!!! question "How many terms should I write on the AP Exam?"
    The AP Exam will in general ask you to write the first four terms of a Taylor Series. 

## MacLaurin Series
The MacLaurin Series is a special case of the Taylor Series, where the center of the series is at $x=0$. The MacLaurin Series is defined as:

$$
f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(0)}{n!}x^n
$$

!!! example "Polynomial Definition of $e^x$"
    To find the derivative of $e^x$ is always $e^x$. Therefore, the derivative of $e^x$ at $x=0$ is always $1$. Using the MacLaurin Series definition, we can write the MacLaurin Series for $e^x$ as:

    $$
    e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!}
    $$

!!! example "Polynomial Definition of $sin(x)$"
    To find the derivative of $sin(x)$ is always $cos(x)$. Therefore, the derivative of $sin(x)$ at $x=0$ alternates between $0$ and $1$. This leaves us with an alternating series of only terms where $n$ is an odd number. Using the MacLaurin Series definition, we can write the MacLaurin Series for $sin(x)$ as:

    $$
    sin(x) = \sum_{n=0}^{\infty} \frac{(-1)^n x^{2n+1}}{(2n+1)!}
    $$