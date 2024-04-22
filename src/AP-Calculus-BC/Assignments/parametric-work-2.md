# Parametric Work 2

1. A very fast bug walks counterclockwise around the edge of a circular table. At time $t = 0$, the bug starts at the point $(3,0)$ and walks 3 feet/second. After one second, what is the bug's angle from the bug's starting point from the center of the circle to the current position (i.e. the central angle)? 2 seconds? $t$ seconds?

    $$
    C = 2\pi r = 2\pi(3) = 6\pi \\
    $$

    Therefore, it takes $2 \pi$ seconds to walk around the edge of the table. Since $2 \pi$ radians is 360 degrees, the bug walks at a rate of 1 radian per second. 

    - After 1 second, the bug is at $\theta = 1$ radian
    - After 2 seconds, the bug is at $\theta = 2$ radians
    - After $t$ seconds, the bug is at $\theta = t$ radians.

2. (continued) What's the bug's x and y coordinates after t seconds?

    $$
    \begin{align*}
    x(t) &= 3\cos(t) \\
    y(t) &= 3\sin(t)
    \end{align*}
    $$

3. Consider the curves $x(t) = 3\cos(t)$ and $y(t) = 3\sin(t)$. Change some values to see what happens and try to explain why those things might occur

    $$
    \begin{align*}
    x(t) &= r_x\cos(a_xt) \\
    y(t) &= r_y\sin(a_yt)
    \end{align*}
    $$

    Observations Noted from $t \in [0, 2\pi]$:

    - $r_x$ and $r_y$ determine the width and height of the parametric curve
    - If you double $a_x$ and $a_y$, you get the number of times the curve crosses the x and y-axes

4. Consider two parametric equations: $x(t) = t^2$, $y(t) = t^4$ and $x(t) = t^3$, $y(t) = t^6$, both from $-5 \leq t \leq 5$. What is the same or different?

    $$x(t) = t^2 \quad y(t) = t^4$$

    <iframe src="https://www.desmos.com/calculator/vjgjvcagay?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

    $$ x(t) = t^3 \quad y(t) = t^6 $$

    <iframe src="https://www.desmos.com/calculator/fyfb04uaaa?embed" width="500" height="500" style="border: 1px solid #ccc" frameborder=0></iframe>

    The same line is traced out by both parametric equations, but the second one is much faster, as the curve is goes to greater values with the same values bounds of $t$. $x(t) = t^3$, $y(t) = t^6$ also has a negative x-axis, while $x(t) = t^2$, $y(t) = t^4$ does not. 

5. Consider $x(t)=tcos(t)$, $y(t)=tsin(t)$ for $0 \le t \le 4 \pi$. What graph do you make here? Why does that happen?

6. $f(x)=cos^{-1}(t)$, $y=sin^{-1}(t)$, then what is y(x) without any trigonometric functions sin^{-1}(cos~x)? [i.e.not~y=

7. Finn the Human is riding his bike and runs aver a piece of gum on one of his 30-inch wheels. Assume that he's riding such that the wheel makes one revolution per second. Also assume that at t=0 is when the gum is on the very bottom of the wheel. Draw a graph of the path that the gum would take as the wheel rolls along a flat surface. (This graph is very special, called a cycloid).

8. (continued) To help find the parametric equation for the cycloid, first assume the wheel is just spinning without any translation (or "transcription"...] Use the diagram to help you (note the spin is clockwise since we eventually want to move to the right):

a. What are the x and y coordinates at t=0,.25,0.5,0.75, and 17

b. Can you find an equation for the y-coordinate as a function of

time? X-coordinate? c. After one second, there's been one revolution. How far does the center move? 2 seconds? t seconds?

d. What is the parametric equation for the cycloid? Make a nice graph (on Desmos probably)
