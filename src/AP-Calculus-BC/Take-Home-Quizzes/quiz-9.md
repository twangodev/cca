# Volume Ratios

This take home quiz will revolve around volumes and the cylinder that it is taken from (also, did you notice the pun?)

1. Let the function $f(t) = at$ where $a$ is a positive real number. If we revolve the area under the curve from $0 \leq t \leq x$, where x is a positive real number, around the x-axis, it will create a familiar shape. Draw a sketch of this situation on a set of axes. What is the volume of this solid, in terms of $x$?
2. Now consider the cylinder that is created when revolving the region under the constant function $y=f(x)$ (where is the function from before) in the first quadrant around the x-axis. Draw this cylinder on the same set of axes as before. What is the ratio of the volume of the familiar shape to the cylinder? (Hint: You should recognize that you just proved a formula from geometry).
3. Now let $g(t)=at^3$. Find the ratio of the solid formed when revolving the region under $g(t)$ from $0 \leq t \leq x$ around the x-axis to the cylinder that it "sits" in.
4. Let $h(t) = a \sqrt{t}$. Do the same thing as the previous question.
5. Show that for any power function of the form $f(t) = at^k$, where $a$ and $k$ are positive real numbers, that the ratio of the volume and the cylinder that it "sits" in is always a constant.

Let $V(x)$ be the volumes that you found before and $C(x)$ be the cylinders that you used before. You've shown $\frac{V(x)}{C(x)}$ should be constant for power functions. Now we're going to prove a more interesting result.

1. Let $y =  f$ be a positive, increasing, twice-differentiable function. Let $\frac{V(x)}{C(x)} = Q$, which is a constant Q. Differentiate both sides to show that $V = \frac{cv'}{c'}$
2. Use $C(x)=\pi x\cdot f^2(x)$ and $V(x) = \int_0^x \pi f^2(t) dt$. What is $V'$?
3. Let $y=f(x)$. If $V = \frac{cv'}{c'}$, show by implicit differentiation that $y^2= \frac{(y+2xy')(3xy^2y'+y^3)-(xy^3)(3y'+2xy'')}{(y+2xy')^2}$
4. Now show that the above simplifies to $xyy'' - xy'^2$
5. Divide both sides by $xyy'$ and then integrate. (Hint: If you're confused, use a u-sub)
6. Solve the result for $\frac{y'}{y} and then integrate again. You should have shown something interesting about power functions.