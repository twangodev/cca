# Final Cheat Sheet

## Inverse Variation

### Classifying Equations

- None: $ x $ not applicable
- Direct: $ ax $ (where $ a $ is a constant)
- Inverse: $ \frac{a}{x} $ (where $ x \neq 0 $)

### Classifying Data

- None: $ xy $ and $ \frac{y}{x} $ are not constant
- Direct: $ \frac{y}{x} $ is constant
- Inverse: $ xy $ is constant

## Graphing Rational Functions

### Rational Function Form

A rational function can be expressed as $ f(x) = \frac{p(x)}{q(x)} $

#### Simple Rational Function: $ y = \frac{a}{x} $

1. Has the same asymptotes, domain, and range as $ f(x) = \frac{1}{x} $
2. Graphing Translations with $ y = \frac{a}{(x−h)} + k $

    - **Step 1:** Draw the asymptotes $ x = h $ and $ y = k $
    - **Step 2:** Plot points to the left and to the right of the vertical asymptote
    - **Step 3:** Draw the two branches of the hyperbola so that they pass through the plotted points and approach the asymptotes

#### Other Rational Functions: $ y = \frac{ax + b}{cx + d} $

1. Vertical Asymptote: $ x = -\frac{d}{c} $
2. Horizontal Asymptote: $ y = \frac{a}{c} $
3. Convert $ y = \frac{ax + b}{cx + d} $ to $ y = \frac{a}{(x−h)} + k $ using long division or synthetic division

## Multiplying and Dividing Rational Expressions

### Rational Expression

A fraction whose numerator and denominator are nonzero polynomials

### Simplified Form

When a rational expression's numerator and denominator have no common factors

### Simplifying Rational Expressions

$ \frac{ac}{bc} = \frac{a}{b} $ when $ ac $ and $ bc $ are not zero.

- **Tip:** Factor the polynomial to find common factors

### Multiplying Rational Expressions

$ \frac{a}{b} \times \frac{c}{d} = \frac{ac}{bd} $ (where $ b,d \neq 0 $)

- **Tip:** Factor the polynomials to find common factors to simplify

### Dividing Rational Expressions

$ \frac{a}{b} \div \frac{c}{d} = \frac{ad}{bc} $ (where $ b,c,d \neq 0 $)

- **Tip:** Factor the polynomials to find common factors to simplify

## Adding and Subtracting Rational Expressions

### Adding and Subtracting with Like Denominators

- **Addition:** $ \frac{a}{c} + \frac{b}{c} = \frac{a+b}{c} $ (where $ c \neq 0 $)
- **Subtraction:** $ \frac{a}{c} - \frac{b}{c} = \frac{a-b}{c} $

### Adding and Subtracting with Unlike Denominators

- **Addition:** $ \frac{a}{c} + \frac{b}{d} = \frac{ad + bc}{cd} $
- **Subtraction:** $ \frac{a}{c} - \frac{b}{d} = \frac{ad - bc}{cd} $

## Solving Rational Equations

For the equation $ \frac{a}{b} = \frac{c}{d} $, cross multiplication gives us:

$$
ad = bc
$$

## Defining and Using Sequences and Series

### Sequence
A sequence is an ordered list of numbers where:

- **Domain**: Relative position of each term.
- **Range**: Terms of the sequence.

### Series
A series is when the terms of a sequence are added together.

#### Summation Notation (Sigma Notation)
Summation notation is used to write a series compactly:

- **Symbol**: ∑
- **Name**:
    - **a**: Upper limit of Summation
    - **b**: Index of Summation
    - **c**: Lower limit of summation
    - **d**: Rule

The general form is:

$$ \sum_{b=c}^{a} d $$

#### Formulas for Special Series
Formulas for the sum of special series include:

- **Sum of n terms of 1**:

$$ \sum_{i=1}^{n} 1 = n $$

- **Sum of first n positive integers**:

$$ \sum_{i=1}^{n} i = \frac{n(n+1)}{2} $$

- **Sum of squares of first n positive integers**:

$$ \sum_{i=1}^{n} i^2 = \frac{n(n+1)(2n+1)}{6} $$

## Analyzing Arithmetic Sequences and Series

### Arithmetic Sequence
An arithmetic sequence is where the difference between consecutive terms is constant, known as the common difference (d).

- **Testing if a sequence is arithmetic**:

$$ d = a_{n+1} - a_n $$

(d should be constant)

- **Rule for Arithmetic Sequences**:

$$ a_n = a_1 + (n-1)d $$

Where:
- **a_n**: The nth term
- **a_1**: The first term
- **d**: The common difference

### Arithmetic Series
An arithmetic series is the expression formed by adding the terms of an arithmetic sequence.

- **The Sum of a Finite Arithmetic Series**:

$$ S_n = \frac{n(a_1 + a_n)}{2} $$

## Analyzing Geometric Sequences and Series

### Geometric Sequence
A geometric sequence is where the ratio of any term to the previous term is constant, known as the common ratio (r).

- **Testing if a sequence is geometric**:

$$ r = \frac{a_{n+1}}{a_n} $$

(r should be constant)

- **Rule for Geometric Sequences**:

$$ a_n = a_1 r^{(n-1)} $$

Where:
- **a_n**: The nth term
- **a_1**: The first term
- **r**: The common ratio

### Geometric Series
A geometric series is the expression formed by adding the terms of a geometric sequence.

- **The Sum of a Finite Geometric Series**:

$$ S_n = a_1 \frac{(1-r^n)}{(1-r)}; \quad r \neq 1 $$

## Finding Sums of Infinite Geometric Series

### Partial Sum
A partial sum, $ S_n $, is the sum to the first n terms of an infinite series (which may be approaching a limiting value).

### The Sum of an Infinite Geometric Series
The sum of an infinite geometric series, when $ |r| < 1 $, is given by:

$$ S = \frac{a_1}{(1-r)} $$

## Using Recursive Rules with Sequences

### Explicit Rule
An explicit rule gives $ a_n $ as a function of the term's position n in the sequence.

### Recursive Rule
A recursive rule provides the beginning term(s) of a sequence and an equation that relates each term to the previous term(s).

#### Recursive Equations for Arithmetic and Geometric Sequences

- **Arithmetic Sequence**:

$$ a_n = a_{n-1} + d $$

- **Geometric Sequence**:

$$ a_n = r \cdot a_{n-1} $$

By using these rules and formulas, various types of sequences and series can be analyzed and their sums can be calculated.
## Defining and Using Sequences and Series

### Sequence
A sequence is an ordered list of numbers where:

- **Domain**: Relative position of each term.
- **Range**: Terms of the sequence.

### Series
A series is when the terms of a sequence are added together.

#### Summation Notation (Sigma Notation)
Summation notation is used to write a series compactly:

- **Symbol**: ∑
- **Name**:
    - **a**: Upper limit of Summation
    - **b**: Index of Summation
    - **c**: Lower limit of summation
    - **d**: Rule

The general form is:

$$ \sum_{b=c}^{a} d $$

#### Formulas for Special Series
Formulas for the sum of special series include:

- **Sum of n terms of 1**:

$$ \sum_{i=1}^{n} 1 = n $$

- **Sum of first n positive integers**:

$$ \sum_{i=1}^{n} i = \frac{n(n+1)}{2} $$

- **Sum of squares of first n positive integers**:

$$ \sum_{i=1}^{n} i^2 = \frac{n(n+1)(2n+1)}{6} $$

## Analyzing Arithmetic Sequences and Series

### Arithmetic Sequence
An arithmetic sequence is where the difference between consecutive terms is constant, known as the common difference (d).

- **Testing if a sequence is arithmetic**:

$$ d = a_{n+1} - a_n $$

(d should be constant)

- **Rule for Arithmetic Sequences**:

$$ a_n = a_1 + (n-1)d $$

Where:
- **a_n**: The nth term
- **a_1**: The first term
- **d**: The common difference

### Arithmetic Series
An arithmetic series is the expression formed by adding the terms of an arithmetic sequence.

- **The Sum of a Finite Arithmetic Series**:

$$ S_n = \frac{n(a_1 + a_n)}{2} $$

## Analyzing Geometric Sequences and Series

### Geometric Sequence
A geometric sequence is where the ratio of any term to the previous term is constant, known as the common ratio (r).

- **Testing if a sequence is geometric**:

$$ r = \frac{a_{n+1}}{a_n} $$

(r should be constant)

- **Rule for Geometric Sequences**:

$$ a_n = a_1 r^{(n-1)} $$

Where:
- **a_n**: The nth term
- **a_1**: The first term
- **r**: The common ratio

### Geometric Series
A geometric series is the expression formed by adding the terms of a geometric sequence.

- **The Sum of a Finite Geometric Series**:

$$ S_n = a_1 \frac{(1-r^n)}{(1-r)}; \quad r \neq 1 $$

## Finding Sums of Infinite Geometric Series

### Partial Sum
A partial sum, $ S_n $, is the sum to the first n terms of an infinite series (which may be approaching a limiting value).

### The Sum of an Infinite Geometric Series
The sum of an infinite geometric series, when $ |r| < 1 $, is given by:

$$ S = \frac{a_1}{(1-r)} $$

## Using Recursive Rules with Sequences

### Explicit Rule
An explicit rule gives $ a_n $ as a function of the term's position n in the sequence.

### Recursive Rule
A recursive rule provides the beginning term(s) of a sequence and an equation that relates each term to the previous term(s).

#### Recursive Equations for Arithmetic and Geometric Sequences

- **Arithmetic Sequence**:

$$ a_n = a_{n-1} + d $$

- **Geometric Sequence**:

$$ a_n = r \cdot a_{n-1} $$

By using these rules and formulas, various types of sequences and series can be analyzed and their sums can be calculated.

## Right Triangle Definitions of Trigonometric Functions

In a right triangle, the trigonometric functions are defined as follows:

- Sine of angle $ \theta $: $ \sin(\theta) = \frac{\text{Opposite}}{\text{Hypotenuse}} $
- Cosine of angle $ \theta $: $ \cos(\theta) = \frac{\text{Adjacent}}{\text{Hypotenuse}} $
- Tangent of angle $ \theta $: $ \tan(\theta) = \frac{\text{Opposite}}{\text{Adjacent}} $

The reciprocal trigonometric functions are defined as:

- Cosecant of angle $ \theta $: $ \csc(\theta) = \frac{\text{Hypotenuse}}{\text{Opposite}} = \frac{1}{\sin(\theta)} $
- Secant of angle $ \theta $: $ \sec(\theta) = \frac{\text{Hypotenuse}}{\text{Adjacent}} = \frac{1}{\cos(\theta)} $
- Cotangent of angle $ \theta $: $ \cot(\theta) = \frac{\text{Adjacent}}{\text{Opposite}} = \frac{1}{\tan(\theta)} $

## Angles and Radian Measure

### Standard Position

An angle is in standard position when its vertex is at the origin and its initial side lies on the positive x-axis.

### Coterminal Angles

Coterminal angles are those whose terminal sides coincide.

### Radian Measure

A radian is the measure of an angle in standard position whose terminal side intercepts an arc of length equal to the radius of the circle.

### Converting Between Degrees and Radians

- Degrees to Radians: Multiply by $ \frac{\pi}{180} $
- Radians to Degrees: Multiply by $ \frac{180^\circ}{\pi} $

### Sector and Central Angle

A sector is a region of a circle that is bounded by two radii and an arc of the circle. The central angle $ \theta $ is the angle formed by the sector.

### Arc Length and Area of Sector

- Arc Length: $ s = r\theta $
- Area of a Sector: $ A = \frac{1}{2} r^2 \theta $

## Trigonometric Functions of Any Angle

### General Definitions of Trigonometric Functions

For a point (x,y) on the terminal side of an angle $ \theta $ in standard position with $ r $ being the distance from the origin to the point, the trigonometric functions are defined as:

- $ \sin(\theta) = \frac{y}{r} $
- $ \csc(\theta) = \frac{r}{y} $ (with $ y \neq 0 $)
- $ \cos(\theta) = \frac{x}{r} $
- $ \sec(\theta) = \frac{r}{x} $ (with $ x \neq 0 $)
- $ \tan(\theta) = \frac{y}{x} $ (with $ x \neq 0 $)
- $ \cot(\theta) = \frac{x}{y} $ (with $ y \neq 0 $)

### Unit Circle

The unit circle is defined by the equation $ x^2 + y^2 = 1 $ and has a center at (0,0) with a radius of 1.

### Quadrantal Angles

Quadrantal angles are angles in standard position whose terminal side lies on an axis.

### Reference Angle Relationships

Reference angles for different quadrants are calculated as follows:

- Quadrant 2 (Top Left): $ 180^\circ - \theta $ or $ \pi - \theta $
- Quadrant 3 (Bottom Left): $ \theta - 180^\circ $ or $ \theta - \pi $
- Quadrant 4 (Bottom Right): $ 360^\circ - \theta $ or $ 2\pi - \theta $

### Evaluating Trigonometric Functions

The sign of trigonometric functions in different quadrants is as follows:

#### Quadrant II

- $ \sin(\theta) $, $ \csc(\theta) $ are positive
- $ -\cos(\theta) $, $ -\sec(\theta) $ are negative
- $ -\tan(\theta) $, $ -\cot(\theta) $ are negative

#### Quadrant I

- $ \sin(\theta) $, $ \csc(\theta) $ are positive
- $ \cos(\theta) $, $ \sec(\theta) $ are positive
- $ \tan(\theta) $, $ \cot(\

theta) $ are positive

#### Quadrant III

- $ -\sin(\theta) $, $ -\csc(\theta) $ are negative
- $ -\cos(\theta) $, $ -\sec(\theta) $ are negative
- $ \tan(\theta) $, $ \cot(\theta) $ are positive

#### Quadrant IV

- $ -\sin(\theta) $, $ -\csc(\theta) $ are negative
- $ \cos(\theta) $, $ \sec(\theta) $ are positive
- $ -\tan(\theta) $, $ -\cot(\theta) $ are negative

## Graphing Sine and Cosine Functions

### Characteristics of $ y = \sin(x) $ and $ y = \cos(x) $

- Domain: All real numbers
- Range: $ -1 \leq y \leq 1 $
- Amplitude: 1
- Period: $ 2\pi $

### Amplitude and Period

For functions $ y = a \sin(bx) $ and $ y = a \cos(bx) $:

- Amplitude: $ |a| $
- Period: $ \frac{2\pi}{|b|} $

### Phase Shift

A phase shift is a horizontal translation of a periodic function.

### Graphing

1. Identify amplitude $ a $, period $ \frac{2\pi}{b} $, horizontal shift $ h $, and vertical shift $ k $ of the graph.
2. Draw the horizontal line $ y = k $.
3. Find the five key points by translating horizontally $ h $ units and vertically $ k $ units.
4. Draw the graph through the translated key points.

## Graphing Other Trigonometric Functions

### Characteristics of $ y = \tan(x) $ and $ y = \cot(x) $

- Domain:
   - $ \tan(x) $: All real numbers except odd multiples of $ \frac{\pi}{2} $
   - $ \cot(x) $: All real numbers except multiples of $ \pi $
- Range: All real numbers
- Period: $ \pi $

### Period and Vertical Asymptotes

For functions $ y = a \tan(bx) $ and $ y = a \cot(bx) $:

- Period: $ \frac{\pi}{b} $
- Vertical Asymptotes:
   - $ y = a \tan(bx) $: Odd multiples of $ \frac{\pi}{|b|} $
   - $ y = a \cot(bx) $: Multiples of $ \frac{\pi}{|b|} $

### Characteristics of $ y = \sec(x) $ and $ y = \csc(x) $

- Domain:
   - $ y = \sec(x) $: All real numbers except odd multiples of $ \frac{\pi}{2} $
   - $ y = \csc(x) $: All real numbers except multiples of $ \pi $
- Range: $ y \leq -1 $ or $ y \geq 1 $
- Period: $ 2\pi $

## Modeling with Trigonometric Functions

### Frequency
The number of cycles that occur per unit of time is known as the *frequency*. It is mathematically described as the reciprocal of the period (T), which is the duration of one complete cycle.

### Sinusoids
Sinusoids are the graphs that represent sine and cosine functions. These functions model periodic phenomena.

#### Writing sine and cosine functions
To write sine and cosine functions, one must determine the values of $ a $, $ b $, $ h $, and $ k $ where the general form is:
- $ y = a \sin(b(x - h)) + k $
- $ y = a \cos(b(x - h)) + k $

Here, $ a $ represents amplitude, $ b $ is related to the frequency, $ h $ is the horizontal shift (phase shift), and $ k $ is the vertical shift.

## Using Trigonometric Identities

### Trigonometric Identity
A trigonometric identity is an equation involving trigonometric functions that is true for every value of the variable for which both sides of the equation are defined.

### Fundamental Trigonometric Identities

#### Reciprocal Identities

$$
\csc(\theta) = \frac{1}{\sin(\theta)}, \quad \sec(\theta) = \frac{1}{\cos(\theta)}, \quad \cot(\theta) = \frac{1}{\tan(\theta)}
$$

#### Tangent and Cotangent Identities

$$
\tan(\theta) = \frac{\sin(\theta)}{\cos(\theta)}, \quad \cot(\theta) = \frac{\cos(\theta)}{\sin(\theta)}
$$

#### Pythagorean Identities

$$
\sin^2(\theta) + \cos^2(\theta) = 1, \quad 1 + \tan^2(\theta) = \sec^2(\theta), \quad 1 + \cot^2(\theta) = \csc^2(\theta)
$$

#### Cofunction Identities

$$
\sin\left(\frac{\pi}{2} - \theta\right) = \cos(\theta), \quad \cos\left(\frac{\pi}{2} - \theta\right) = \sin(\theta), \quad \tan\left(\frac{\pi}{2} - \theta\right) = \cot(\theta)
$$

#### Negative Angle Identities

$$
\sin(-\theta) = -\sin(\theta), \quad \cos(-\theta) = \cos(\theta), \quad \tan(-\theta) = -\tan(\theta)
$$

## Using Sum and Difference Formulas

### Sum Formulas

$$
\sin(a + b) = \sin(a)\cos(b) + \cos(a)\sin(b)
$$

$$
\cos(a + b) = \cos(a)\cos(b) - \sin(a)\sin(b)
$$

$$
\tan(a + b) = \frac{\tan(a) + \tan(b)}{1 - \tan(a)\tan(b)}
$$

### Difference Formulas

$$
\sin(a - b) = \sin(a)\cos(b) - \cos(a)\sin(b)
$$

$$
\cos(a - b) = \cos(a)\cos(b) + \sin(a)\sin(b)
$$

$$
\tan(a - b) = \frac{\tan(a) - \tan(b)}{1 + \tan(a)\tan(b)}
$$