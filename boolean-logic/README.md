# Control Flow in JavaScript - Boolean Logic

![Hero image](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

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

## Relational Operators

JavaScript also has a host of relational operators: 

- `<` - Less than
- `>` - Greater than
- `<=` - Less than or equal to
- `>=` - Greater than or equal to

```javascript
3 < 4       // true
3 > 4       // false
10 >= 5 + 5 // true
```

## Logical Operators

The logical operators `||` and `&&` are more powerful than meets the eye.

The logical `||` (OR) operator always returns the first operand if it is truthy; otherwise, the second operand is returned:

```javascript
'hello' || 'goodbye'  // evaluates to 'hello'
0 || null  // evaluates to null
```

The logical `&&` (AND) operator always returns the first operand if it is falsy, otherwise the second operand will be returned:

```javascript
'hello' && 'goodbye'  // evaluates to 'goodbye'
0 && null  // evaluates to 0
```

## The Not Operator

The __not operator__ (`!`), also known as the “bang” operator, flips a `true` or truthy expression to the boolean value of false, and vice-versa. For example: 

```javascript
!false  // true
!null   // true
!3      // false
!''     // true
```

When used in conjunction with the equality operators, the syntax looks like this: 
- `!==` - Strict Inequality
- `!=` - Loose Inequality

```javascript
3 !== 4   // true, 3 isn't equal to 4
3 != '3'  // false, 3 is loosely equal to '3'
```

As the bang operator converts a truthy or falsy operand to a flipped boolean value, 
a double `!` operator is a great way to force an expression into its actual boolean value of true or false. For example: 

```javascript
!!3   // true
```
The first `!` converts `3` to `false`, then the second `!` converts `false` to `true`. 

