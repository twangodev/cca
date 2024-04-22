# For Loop

```java
for (<init>, <predicate>, <update-expr>) { <body> }
```

## Evaluation Procedure

1. `<init>` is run once, only at the beginning
2. `<predicate>` is evaluated, if `false`, the for loop execution stops
3. `<body>` is executed
4. `<update-expr>` is executed
5. Repeat from Step 2

!!! tip
    When the `break` keyword is evaluated, the loop exists immediately

## Scope

A new frame is created during execution of the `<body>`

!!! tip
    Uninitialized variables outside the scope of body can be initialized within the child frame (local scope), but do not effect the parent frame (global scope)


## While Loops

```java
while (<condition>) { <body> }
```

### Evaluation Procedure

1. `<condition>` is evaluated, if `true`, `<body>` is executed
2. Repeat step 1

### Do/While Loops

```java
do { <body> } while (<condition>);
```
#### Evaluation Procedure

1. `<body>` is executed, and `<condition>` is checked
2. If `<condition>` is `true`, then repeat step 1