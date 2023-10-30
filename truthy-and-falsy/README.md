# ![JavaScript Control Flow - Truthy and Falsy](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will understand the concept of truthy/falsy values. 

## Truthy and Falsy

JavaScript has the primitive `boolean` values of `true` and `false`, but it also has the idea of ***truthy*** and ***falsy***. So what are truthy and falsy, and why don't we use `true` and `false` for everything?

Truthy and falsy are conceptual and attempt to treat non-boolean expressions as booleans (`true` or `false`) during runtime. 

Most things in JavaScript are truthy, so it's easier to remember what is falsy:

These two data types are always falsy:
  
- `null`
- `undefined`

These four values are falsy: 

- `false`
- `0` (zero)
- `NaN` (Not a Number)
- `''` (An empty string. A string with a value of a space (`' '`) is not empty.)

Everything else is truthy!

The concept of truthiness/falsyness will often allow us to write less code. It ensures that we can write conditions that check a value itself rather than what that value would equal.

Because this concept allows less code to be written, you'll often see code that takes advantage of this in the wild. Note that this can lead to pitfalls if you're not absolutely sure what the possible values of data you're working with are, so most course content does not take advantage of truthiness or faslyness. 

For instance, since an empty string is falsy, you can check a variable in a condition: 

```javascript
let string = "truthy value";

if (string) {
  // do some stuff because this is not an empty string
}
```

Rather than having to evaluate the value of the variable: 

```javascript
if (string !== "") {
  // this is a more lengthy way of trying to make the same check without 
  // relying on the inherent nature of truthy/falsy values in JavaScript
}
```
