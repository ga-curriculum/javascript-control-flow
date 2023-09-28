# Control Flow in JavaScript - Level Up - 'break' and 'continue' Statements

![Hero image](./assets/hero.png)

The [break](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/break) statement is used to immediately exit a `while` or `for` loop. For example: 

```javascript
let word = '';
let words = [];
while (true) {
  word = prompt('Enter a word ("end" to quit)');
  if (word === 'end') break;
  words.push(word);
  console.log("You've entered: " + words.join(', '));
}
```

The [continue](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/continue) statement skips remaining code in the current iteration and returns to the top of the `while` or `for` loop.
