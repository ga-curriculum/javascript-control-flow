# ![Control Flow in JavaScript - Boolean Logic](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to use comparison operators to evaluate operands. 

## Equality operators

Equality operators are used to compare the values of left and right operands, which can be variables, literal values, and more.

There are two primary equality comparison operators in JavaScript: 
- `===` - strict equality (best practice)
- `==` - loose equality (performs type conversion)

The strict equality operator (commonly called 'triple equals') compares the values of the left and right operands and returns `true` if they have the same value. 

If the values have different types, then the operator returns `false`. 

```javascript
3 === 3   // true
3 === 4   // false
3 === '3' // false 
```

We'll always use strict equality as a best practice. You can read more about loose equality in the [Loose Equality Level Up](../level-up/loose-equality.md).

## Relational operators

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

## Logical operators

The logical operators `||` and `&&` help evaluate multiple conditions simultaneously.

The logical OR (`||`) operator evaluates multiple conditions. If any of the conditions evaluate to `true`, then the operator resolves to `true`. Here are some examples:

```javascript
true || true   // true
true || false  // true
false || false // false

'sandwich' === 'sandwich' || 2 === 2 // true
'hotdog' === 'sandwich' || 2 === 2   // true
'hotdog' === 'sandwich' || 4 === 5   // false
```

More than two conditions may be evaluated at a time. For example:

```js
true || true || true    // true
true || true || false   // true
true || false || false  // true
false || false || false // false
```

The logical AND (`&&`) operator also evaluates multiple conditions. Every condition must evaluate to `true` for the operator to resolve to `true`. Using the same examples as above, and only changing the operator:

```javascript
true && true   // true
true && false  // false
false && false // false

'sandwich' === 'sandwich' && 2 === 2 // true
'hotdog' === 'sandwich' && 2 === 2   // false
'hotdog' === 'sandwich' && 4 === 5   // false
```

Again, more than two conditions may be evaluated at a time. For example:

```js
true && true && true    // true
true && true && false   // false
true && false && false  // false
false && false && false // false
```

## The not operator

The not (`!`) operator, also known as the bang operator, flips a `true` expression to the boolean value of `false`, and vice-versa. For example: 

```javascript
!false  // true
!true   // false
```

When used in conjunction with the equality operators, the syntax looks like this: 
- `!==` - Strict Inequality

```javascript
3 !== 4   // true, 3 isn't equal to 4
3 !== 3   // false, 3 is equal to 3
```
