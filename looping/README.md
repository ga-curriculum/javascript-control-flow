# Control Flow in JavaScript - Looping

![Hero image](./assets/hero.png)

**Learning objective:** By the end of this lesson, students will be able to tktk

Looping is a control flow mechanism that will repeat a set of actions until a condition is met or while a condition is truthy.

Looping statements allow us to execute a block of code multiple times, and are a fundamental part of working with collections of data like arrays. 

## for

A for loop repeats until a specific condition evaluates to false. 

The syntax is as follows: 

```javascript
for (initialExpression; conditionExpression; incrementExpression) {
  statement
}
```

When a for loop executes, the following occurs:
1. The initializing expression `initialExpression`, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
2. The `conditionExpression` expression is evaluated. If the value of `conditionExpression` is truthy, the loop `statement` executes. If the value of `conditionExpression` is falsy, the `for` loop terminates.
3. The `statement` executes. Use curly brackets (`{ ... }`) to encapsulate the `statement`.
4. The update expression `incrementExpression` is executed.
5. Control returns to Step 2.

<br>

Let's examine the syntax with an example: 

```javascript
for (let number = 1; number < 10; number++) {
	console.log(number)
}
```

1. The `initialExpression` runs only once before looping begins. It is used to declare and initialize a looping variable. In this example, a new variable named `number` is initialized with the value `1`. 
2. The `conditionExpression` will be evaluated before each loop. If truthy, the code block will execute. At the start of this loop, `number` was just initialized as 1, so `number < 10` is truthy. 
3. The `incrementExpression` will execute after each loop. Typically this increments the looping variable by one, but any kind of expression can be used here.

## while

Both the `for` and `while` statements require a conditional expression. `while` loops only specify the `conditionExpression`: 

```javascript
let number = 1
while (number <= 10) {
  console.log(number)
	number++
}
```
Where, `x <= 10` is the conditional expression. 

You'll notice that a `for` loop and a `while` loop work similarly, but where a `for` loop specifies all of the loop parameters up front, a `while` loop allows for more freedom in composition. This is perhaps why `while` loops are especially susceptible to causing __infinite loops__. 

For instance, it would be easy to forget to increment `number`: 
```javascript
let number = 1
while (number <= 10) {
  console.log(number)
}
```

As written, `number` will never be larger than or equal to 10, so this `while` loop will run forever, endlessly logging the number 1 until the end of time (or until we tell it to stop). 


> 🧠 An infinite loop (or endless loop) is a sequence of code that will continue endlessly. 

