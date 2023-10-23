# ![Control Flow in JavaScript - Level Up - Nested Branching Statements](./assets/hero-nested-branching-statements.png)

Sometimes, you'll encounter situations where one condition depends on another. In such cases, you can use nested `if` statements. These are `if` statements placed inside other `if` or `else` blocks, allowing for more complex decision-making. Here's an example:


```js
const dayOfTheWeek = 'Friday';
const isAfternoon = true;

if (dayOfTheWeek === 'Friday') {
  if (isAfternoon) {
    console.log('Almost the weekend!');
  } else {
    console.log('Happy Friday morning!');
  }
} else {
  console.log("It's not Friday.");
}
```

Clarity and simplicity are essential when using branching in your code. Complex nested conditions can be challenging to understand, so use this sparingly. Always strive for readability.
