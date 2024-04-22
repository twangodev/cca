# Final Cheat Sheet

## Inverse Variation

### Classifying Equations

- None: \( x \) not applicable
- Direct: \( ax \) (where \( a \) is a constant)
- Inverse: \( \frac{a}{x} \) (where \( x \neq 0 \))

### Classifying Data

- None: \( xy \) and \( \frac{y}{x} \) are not constant
- Direct: \( \frac{y}{x} \) is constant
- Inverse: \( xy \) is constant

## Graphing Rational Functions

### Rational Function Form

A rational function can be expressed as \( f(x) = \frac{p(x)}{q(x)} \)

#### Simple Rational Function: \( y = \frac{a}{x} \)

1. Has the same asymptotes, domain, and range as \( f(x) = \frac{1}{x} \)
2. Graphing Translations with \( y = \frac{a}{(x−h)} + k \)

  - **Step 1:** Draw the asymptotes \( x = h \) and \( y = k \)
  - **Step 2:** Plot points to the left and to the right of the vertical asymptote
  - **Step 3:** Draw the two branches of the hyperbola so that they pass through the plotted points and approach the asymptotes

#### Other Rational Functions: \( y = \frac{ax + b}{cx + d} \)

1. Vertical Asymptote: \( x = -\frac{d}{c} \)
2. Horizontal Asymptote: \( y = \frac{a}{c} \)
3. Convert \( y = \frac{ax + b}{cx + d} \) to \( y = \frac{a}{(x−h)} + k \) using long division or synthetic division

## Multiplying and Dividing Rational Expressions

### Rational Expression

A fraction whose numerator and denominator are nonzero polynomials

### Simplified Form

When a rational expression's numerator and denominator have no common factors

### Simplifying Rational Expressions

\( \frac{ac}{bc} = \frac{a}{b} \) when \( ac \) and \( bc \) are not zero.

- **Tip:** Factor the polynomial to find common factors

### Multiplying Rational Expressions

\( \frac{a}{b} \times \frac{c}{d} = \frac{ac}{bd} \) (where \( b,d \neq 0 \))

- **Tip:** Factor the polynomials to find common factors to simplify

### Dividing Rational Expressions

\( \frac{a}{b} \div \frac{c}{d} = \frac{ad}{bc} \) (where \( b,c,d \neq 0 \))

- **Tip:** Factor the polynomials to find common factors to simplify

## Adding and Subtracting Rational Expressions

### Adding and Subtracting with Like Denominators

- **Addition:** \( \frac{a}{c} + \frac{b}{c} = \frac{a+b}{c} \) (where \( c \neq 0 \))
- **Subtraction:** \( \frac{a}{c} - \frac{b}{c} = \frac{a-b}{c} \)

### Adding and Subtracting with Unlike Denominators

- **Addition:** \( \frac{a}{c} + \frac{b}{d} = \frac{ad + bc}{cd} \)
- **Subtraction:** \( \frac{a}{c} - \frac{b}{d} = \frac{ad - bc}{cd} \)

## Solving Rational Equations

For the equation \( \frac{a}{b} = \frac{c}{d} \), cross multiplication gives us:

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
A partial sum, \( S_n \), is the sum to the first n terms of an infinite series (which may be approaching a limiting value).

### The Sum of an Infinite Geometric Series
The sum of an infinite geometric series, when \( |r| < 1 \), is given by:

$$ S = \frac{a_1}{(1-r)} $$

## Using Recursive Rules with Sequences

### Explicit Rule
An explicit rule gives \( a_n \) as a function of the term's position n in the sequence.

### Recursive Rule
A recursive rule provides the beginning term(s) of a sequence and an equation that relates each term to the previous term(s).

#### Recursive Equations for Arithmetic and Geometric Sequences

- **Arithmetic Sequence**:

$$ a_n = a_{n-1} + d $$

- **Geometric Sequence**:

$$ a_n = r \cdot a_{n-1} $$

By using these rules and formulas, various types of sequences and series can be analyzed and their sums can be calculated.