# Variables

## Assignment

```java
int x = 0; // Create a variable x, which is bound to 0
```

Variable definition follows the following syntax: `<type> <name> = <binding>;`

### Multiple Declarations

Java supports multi-line definitions

#### Initializing and Binding Variables

```java
double a, b, c; // Pure assignment
double x = 1.1, y = 1.2, z; // only x and y are bound
```

## Primitive Types

In Java, 8 primitive types are supported, and `String` (total 9). Each of these is **immutable**

<aside>
💡 `char` is defined with a single quote

</aside>

<aside>
💡 For precise calculations involving decimals, use `BigDecimal` instead of `float` or `double`, as floating points will result in rounding inaccuracies

</aside>

### Arithmetic

Integer - Integer division will result in a integer, but floored

Other mixed arithmetic operations will covert all of the operands into doubles before dividing

#### Evaluation Rule

Java follows PEMDAS: Parenthesis, Exponents, Multiply, Divide, Add, and Subtract

#### Automatic Flooring

When defining an `int`, Java will automatically floor the calculation

#### Increments

```java
int a = 0;
int b = a++;
System.out.println(a + " " + b); // 1 0
int c = ++a;
System.out.println(a + " " + b + " " + c); // 2 0 2
```

<aside>
💡 Java’s order of evaluation of `a++` will bind `b` to `a`, then perform the `++` operation on `a`, incrementing the value of `a`. Likewise, `++a` will increment, then bind.

</aside>

The operation `--` has the same behavior as `++`, other than the fact that it subtracts

#### Arithmetic Assignments (same behavior as in Python)

`+=`, `-=`, `*=`, `/=`, `%=`

### Doubles

#### `Double` Legalities

When assigning a integer value to a decimal, no error is produced, as Java will automatically covert it to a `Double`. The same goes for `float`

#### `Double` Base 10 Tips

When defining a variable that is equal to $a\times10^b$, one may follow the form `<a>E<b>`

### Booleans

A primitive type that only has two states: `true` and `false`

#### Negation

To negate, or invert, a boolean, use the `!` operator

#### Truth Table