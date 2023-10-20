# ![Control Flow in JavaScript - Level Up - Ternary Operator](./assets/hero-ternary-operator.png)

The ternary operator is ideal when you need to return one of two values depending upon a condition:

```javascript
let message = score > 100 ? "You rock!" : "Keep trying!"
```

The above one line of code replaces this code:

```javascript
let message
if (score > 100) {
  message = "You rock!"
} else {
  message = "Keep trying!"
}
```

The ternary operator can also be used to evaluate one of two expressions, so you can run a method if you’d like:
```javascript
score > 100 ? gameWinner() : gameLoop()
```