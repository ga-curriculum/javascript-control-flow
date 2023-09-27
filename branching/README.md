# Control Flow in JavaScript - Branching

![Hero image](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

Branching is a type of control flow that allows for different code paths to be executed based on specific conditions.

## `if`
__Single Path__

To execute a statement or statements conditionally, use the `if` statement. 

```javascript
if (val === 1) {
	console.log('This code will run only if val equals 1')
}
```

Conditional expressions must be surrounded by parenthesis. If you have only a single statement that needs to execute, you can write that statement without using curly braces (used to define a block statement):

```javascript
if (val === 1) console.log('This code will run only if val equals 1')
```

## `if`...`else`
__Dual Paths__

```javascript
if (val === 1) {
  console.log('val is one')
} else {
  console.log('val is not one')
}
```

## `if`...`else if`...`else`
__Three or more paths__

If you have three or more code paths use `if` with as many `else if` statements as necessary and optionally a final `else`:
```javascript
if (val === 1) {
  console.log('val is one')
} else if (val === 2) {
  console.log('val is two')
} else if (val === 3) {
  console.log('val is three')
} else {
  console.log('not one, two, or three')
}
```

## You Do 🧠

Write an `if` … `else if` … `else` statement that console.logs the following based upon the value of a variable named `color`: 

- If the value is `green`, log `Go`
- If the value is `yellow`, log `Slow`
- If the value is `red`, log `Stop`
- If the value is anything else, log `Whatever`

Hint: Don’t forget to declare and initialize a variable named `color`.
