# Control Flow in JavaScript - Level Up - Truthy, Falsy, and Logical Operators

![Hero image](./assets/hero.png)

The logical operators `||` and `&&` are more powerful than meets the eye.

The logical `||` (OR) operator always returns the first operand if it is truthy; otherwise, the second operand is returned:

```javascript
'hello' || 'goodbye' // evaluates to 'hello'
0 || null            // evaluates to null
```

The logical `&&` (AND) operator always returns the first operand if it is falsy; otherwise, the second operand will be returned:

```javascript
'hello' && 'goodbye' // evaluates to 'goodbye'
0 && null            // evaluates to 0
```
