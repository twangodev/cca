# Introduction to Java

```java
public class Main {
	public static void main(String[] args) { // Main method
		System.out.println("Hello World");
	}	
}
```

A snippet of the Hello World code

## Classes

Classes are often referred to as blueprints in programming. Specifically, they represent data abstractions. Classes are used to create, or “instantiate” objects, which can be updated to represent behaviors and change.

!!! tip
    Java is an object-oriented language, meaning that everything must be contained within a class


When thinking about classes, ask yourself, what does it represent? How does it behave?

## About Java Execution

Source code becomes Java bytecode (has ending of `.class`). Bytecode can run on the Java Virtual Machine (JVM). JVM can run on a majority of platforms

#### Manually Running Java

Compile java files in the command line with `javac`, then execute the generated `.class` file with `java`

!!! tip
    File names must be the same as the class name, otherwise there will be a compilation error


## Differences between `print()` and `println()`

`print()` only appends to the standard output, but `println()` will print on a new line.

!!! tip 
    `println(str);` is equivalent to `print(str + "\n");`

## Strings

### Relevant String Methods

| Signature                        | Description                                                                                                                                   | Return Type |
|----------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------|-------------|
| substring(startIndex, endIndex?) | Returns a substring from startIndex (inclusive) to endIndex (exclusive). If endIndex is not specified, it returns everything after startIndex | String      |
| toLowerCase()                    | Returns a String with all lowercase letters                                                                                                   | String      |
| toUpperCase()                    | Returns a String with all uppercase letters                                                                                                   | String      |
| replace(target, replacement)     | Returns a String which replaces all instances of target with replacement                                                                      | String      |

!!! note 
    Methods that return a `String` will not change the original `String`, as `String` is immutable


### Escape Sequences

Using the backslash character `\`, special characters can be formed

| Sequence | Meaning                          |
|----------|----------------------------------|
| \n       | New line or line-break character |
| \t       | Tab                              |
| \\       | The backslash character \        |

### String Concatenation

```java
System.out.println("Hello" + " " + "World" + 5")
>>> Hello World5
```

Using the `+` operator, different primitive variables can be “added together”

!!! tip
    Concatenation in Java is not dependent on type, unlike Python. This means combining numbers with strings isn’t a problem.

#### Unique Cases

```java
System.out.println("Hi" + 5 + 5); // Hi55
```

```java
System.out.println(1 + 2 + "Three"); // 3Three
```