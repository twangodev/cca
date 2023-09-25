# Random

## `Math.random()`

Returns a pseudorandom `double` generated from `java.util.Random` , from the values 0.0 (inclusive) to 1.0 (exclusive)

## Generating a random `int` between the `[a, b)`

```java
int myRandInt = (int) (Math.random() * (b - a) + a) // Floor the result
```