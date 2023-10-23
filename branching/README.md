# ![Control Flow in JavaScript - Branching](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to compose branching logic statements.

## Branching

Branching is a type of control flow that allows for different code paths to be executed based on specific conditions.

### `if`

***Single Path***

To execute a statement or statements conditionally, use the `if` statement. Conditional expressions must be surrounded by parenthesis.

```js
const val = 1;

if (val === 1) {
  console.log('This code will run only if val equals 1');
}
```

### `if...else`

***Dual Paths***

When using an `if...else` statement, the code inside the `if` block will be executed if the condition evaluates to `true`. If the condition evaluates to `false`, then the code inside the `else` block will be executed. 

```js
if (val === 1) {
  console.log('val is one');
} else {
  console.log('val is not one');
}
```

Check out the [Ternary Operator Level Up](../level-up/ternary-operator.md) for another way to write short dual path branches.

### `if...else if...else`

***Three or more paths***

If you have three or more code paths, use `if` with as many `else if` statements as necessary and optionally a final `else`:

```js
if (val === 1) {
  console.log('val is one');
} else if (val === 2) {
  console.log('val is two');
} else if (val === 3) {
  console.log('val is three');
} else {
  console.log('not one, two, or three');
}
```

## You Do 🧠

First, declare and initialize a variable named `color`.

Then, write a branching statement that console.logs the following based upon the value of `color`: 

- If the value is `green`, log `'Go'`
- If the value is `yellow`, log `'Slow'`
- If the value is `red`, log `'Stop'`
- If the value is anything else, log `'Whatever'`

Manipulate the value of `color` to ensure you're able to log all of the above values.

## `switch`

The `switch` statement can also be used for branching, but is less common than the branching techniques above. Check out the [`switch` Level Up](../level-up/switch.md) for more.
