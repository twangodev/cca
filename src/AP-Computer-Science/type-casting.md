# Type Casting

## Widening Casting

Java will automatically cast smaller types to larger types.

The order for casting is as follows: `byte` → `short` → `char` → `int` → `long` → `float` → `double`

## Narrowing Casting

When converting from a larger type to a smaller type, it must be explicitly stated in Java

### Syntax

```java
int myInt = 10;
double myInt = (double) myInt;
```

## Casting Mechanics and Tricks

To round a `double` to a `int`, add `0.5` to the double, then convert to `int`