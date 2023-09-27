# Control Flow in JavaScript - Truthy and Falsy

![Hero image](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will understand the difference between boolean `true`/`false` and truthy/falsy values. 

JavaScript has the primitive `boolean` values of `true` and `false`, but it also has the idea of __truthy__ and __falsy__. So what are truthy and falsy, and why don't we just use `true` and `false`?

Truthy and falsy are conceptual and attempt to treat non-boolean expressions as booleans (`true` or `false`) during runtime. The concept of truthiness/falsyness will often allow us to write more concise code. 

Most things in JS are truthy, so it's easier to remember what is falsy:
- These two data types are always falsy: 
  `null` and `undefined`
- These four values are falsy: 
  `false`, `0`(zero), `NaN` ('Not a Number' - a special value of number), and `""` (an empty string - note that a string with a value of a space is not empty).

Everything else is truthy!