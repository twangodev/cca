# Logic

##  Logical Operators

| Name | Definition | Symbol | Short Circuiting |
| --- | --- | --- | --- |
| Equals | Whether two elements are equal | == | None |
| And | Whether both elements are true | && | If any elements are false, short-circuit to false |
| Or | Whether any of the elements are true | || | If any elements are true, short-circuit to true |
| Negation | Changes to a different Boolean state | ! | None |

##  De Morgan Laws

###  Formal Definition

$$
\overline{A \cup B} = \overline A \cap \overline B
$$

$$
\overline{A \cap B} = \overline A \cup \overline B
$$

### In Java

```java
// Let a and b be to defined and instantiated booleans
!(a && b) == !a || !b
!(a || b) == !a && !b
```
