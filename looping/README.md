# ![Control Flow in JavaScript - Looping](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to compose `for` and `while` loops.

## Looping

Looping is a control flow mechanism that will repeat a set of actions until a condition is met or while a condition is true. Looping is a fundamental part of working with collections of data.

## `for`

A `for` loop repeats until a specific condition evaluates to `false`. `for` loops are commonly used to run a block of code a specified number of times. The syntax is as follows: 

![`for` loop syntax](./assets/for-syntax.png)

1. The `for` keyword.
2. `initialization` - An expression or variable declaration evaluated once before the loop begins. This is typically used to initialize a counter variable. Variables declared with let are local to the statement.
3. `condition` - An expression to be evaluated before each loop iteration. If this expression evaluates to `true`, the `statement` code is executed. If the expression evaluates to `false`, the `statement` code is not executed.
4. `afterthought` - An expression to be evaluated at the end of each loop iteration. This occurs before the next evaluation of the `condition`. It's generally used to update or increment the counter variable.
5. A code block - contains the code to be executed in the loop.
6. The code to be executed as long as the condition evaluates to `true`.

Next, let's examine the order of operation for a `for` loop, with an example:

```javascript
for (let number = 1; number < 10; number++) {
  console.log(number);
}
```

### Step 1 

The `initialization` runs once before looping begins. It is used to declare and initialize a looping variable - in this example, a new variable named `number` is initialized with the value `1`.

### Step 2

The `condition` expression is evaluated. If `true`, the code block will execute. At the start of this loop, `number` was just initialized as 1, so `number < 10` is `true`. If the value of the `condition` becomes `false` the `for` loop terminates.

### Step 3

The `statement` executes.

### Step 4

The update expression `afterthought` is executed. In this example, `number` is [incremented](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Increment) by 1 whenever the `afterthought` is executed.

### Step 5

Control returns to Step 2.

## You Do 🧠 

Write a `for` loop that iterates from 1 - 20 and logs out whether each number in the range is even or odd.

Sample Output: 
```bash
1 is odd 
2 is even
3 is odd
4 is even
[...]
20 is even
```

Check out this documentation on the [remainder operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Remainder) if you need a hint.

## `while` and `do...while`

Reference the [`while` Level Up](../level-up/while.md) and the [`do...while` Level Up](../level-up/do-while.md) to see some more uncommon ways to loop in JavaScript.
