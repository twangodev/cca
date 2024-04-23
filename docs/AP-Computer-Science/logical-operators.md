# Logical Operators

## The If-Else Statement

```java
if (<condition1>) { 
	<body1> 
} else if (<condition2>) {
	<body2>
} else {
	<body3>
}
```

!!! tip
    Curly braces are not required for one-line if-else statements


### Switch Statements

```java
switch (<expression>) {
	case <case1>: <expr> 
	case <case2>: <expr>
	default: <expr>
```

!!! tip
    Java will jump to the first matching case, and will execute blocks after matching case. To prevent execution of following cases, use `break` at the end of the block.

## Equality

The `==` sign is the default way to check for equality. This is equivalent to the `.equals(obj)` method, which is built-in to all classes (all objects extend the `Object` superclass)