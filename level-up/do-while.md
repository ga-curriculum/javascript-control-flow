# ![Control Flow in JavaScript - Level Up - 'do...while'](./assets/hero-do-while.png)

`do`...`while` loops are very similar to `while` loops, except they force the code block to execute at least once, regardless of the condition being truthy or falsy. 

```javascript
let num = 120;

do {
  console.log(`${num} is even`);
  num += 2;
} while (num <= 10);
```

The code inside the `do...while` loop will execute once, even though `120` is not less than or equal to `10`.
