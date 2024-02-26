# Scanner

A class from `java.util`, and typically used to interact with user input

## Initialization

```java
Scanner kb = new Scanner(System.in); // Gets keyboard input from standard ouput
```

## Common `Scanner` Methods

| Signature  | Description                                                    | Return Type |
|------------|----------------------------------------------------------------|-------------|
| nextInt()  | Returns a integer scanned from the Scanner object              | int         |
| next()     | Returns what the first scanned String` from the Scanner object | String      |
| nextLine() | Returns the whole line scanned from the Scanner object         | String      |

!!! tip
    `nextInt()` does not take scan the new-line character from the `InputStream`. This will result with the next call of `nextLine()` to be the new-line character. A fix for this is to call `nextLine()` again, before the actual `nextLine()` is required
