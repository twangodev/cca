# Strings and Characters

## Interoperability

### `String` and `char`

Converting `String` to `char` and `char` to `String` simply by variable definition will result in an error

```java
char myChar = "A"; // Error
String myString = 'A'; // Error
```

Instead, use the method `.charAt(<index>)` to convert a `String` to `char`

#### Converting Characters to Strings

```java
String myString = "" + 'C'; // Concatentation between String and char is allowed
```

### `int` and `char`

Converting `int` to `char` and back is allowed, and Unicode values will be used

```java
int a = 'A'; // a = 65
char a = (char) 65; // Value must be less than 65,536 (unicode)
```

## String Constant Pool

All string literals are stored as `String` constants in a separate memory area called the String constant pool.

When a new `String` is defined, a variable is placed into the String constant pool, with the variable pointing to the value. However, if another variable with the same name as the original variable is declared, then the new variable points towards the original `String` object

### The `new` Keyword with relation to the String Constant Pool

When a `String` is defined with the `new` keyword, a separate place in memory is allocated for the new string, thus String Constant Pool relations do not apply.