# Control Flow in JavaScript - Boolean Logic

![Hero image](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

JavaScript has the primitive `boolean` values of `true` and `false`, but it also has the idea of __truthy__ and __falsy__. So what are truthy and falsy, and why don't we just use `true` and `false`?

Truthy and falsy are conceptual and attempt to treat non-boolean expressions as booleans (`true` or `false`) during runtime. The concept of truthiness/falsyness will often allow us to write more concise code. 

Most things in JS are truthy, so it's easier to remember what is falsy:
- These two data types are always falsy: 
  `null` and `undefined`
- These four values are falsy: 
  `false`, `0`(zero), `NaN` ('Not a Number' - a special value of number), and `""` (an empty string - note that a string with a value of a space is not empty).

Everything else is truthy!

### The Not Operator

The __not operator__ (`!`), also known as the “bang” operator, flips a `true` or truthy expression to the boolean value of false, and vice-versa. For example: 

```javascript
!false  // true
!null   // true
!3      // false
!''     // true
```

As the bang operator converts a truthy or falsy operand to a flipped boolean value, 
a double `!` operator is a great way to force an expression into its actual boolean value of true or false. For example: 

```javascript
!!3   // true
```
The first `!` converts `3` to `false`, then the second `!` converts `false` to `true`. 


## Equality Operators

Comparison operators are used to compare the values of left and right operands, which can be variables, literal values, object properties, etc.

There are two primary equality comparison operators in JavaScript: 
- `===` - Strict Equality (best practice)
- `==` - Loose Equality (performs type conversion)


The strict equality operator (commonly called 'triple equals') compares the values of the left and right operands and returns `true` if they have the same value. 

If the values have different types, then the operator returns `false`. 

```javascript
3 === 3   // true
3 === 4   // false
3 === '3' // false 
```

The loose equality operator (commonly called 'double equals') will perform a type conversion (if needed) when it compares its left and right operands: 

```javascript
3 == '3'  // true
```

In the above example, JavaScript will [coerce](https://developer.mozilla.org/en-US/docs/Glossary/Type_coercion) the string `'3'` into the number 3. Then, JavaScript will perform a strict equality check now that the types are the same:

```javascript
3 === 3
```

3 is strictly equal to 3, so this returns `true`.

Typically, it is best to avoid using the double equals operator - we will rarely be in a position where the type of our data is irrelevant or interchangeable. Use strict equality/triple equals as best practice!


