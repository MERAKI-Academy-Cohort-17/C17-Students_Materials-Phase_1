 # W01D03- Functions In JavaScript Cheat Sheet

## What Are Functions?
- A function is a reusable block of code designed to perform a specific task.


- Calling (invoking) a function is done by using its name followed by parentheses ().

## Function Syntax Overview
- function → Keyword to declare a function.


- () → Place for parameters (input placeholders).


- {} → Holds the executable code.

## Ways to Define Functions
1. Function Declaration:
```js
function greet() {
  console.log("Hello");
};
```

2. Function Expression:
```js
const greet = function () {
  console.log("Hello");
};
```
---

## Parameters vs Arguments
Parameters: Named placeholders in function definition.


Arguments: Actual values passed to a function during invocation.
```js
const intro = function (name, age) {
  console.log("Hi, I'm " + name + " and I'm " + age + " years old.");
};


intro("John", 20);
```
---
## Return Values
Use return to send a value out of a function for use elsewhere.
```js
const add = function (a, b) {
  return a + b;
};
const result = add(10, 5); // result is 15
```


Note: If you don't use return, the function returns undefined.
## Built-in Functions
- console.log() → Prints to the console.


- Math.round(1.6) → Returns 2


- Math.floor(2.7) → Returns 2


- Math.pow(2, 3) → Returns 8


- Math.random() → Returns a random number between 0 and 1


- "text".toUpperCase() → Converts string to uppercase

## Random Functions
```js
const upperCase = function (string) {
  return string.toUpperCase();
};


const average = function (a, b) {
  return (a + b) / 2;
};


const floor = function (number) {
  return Math.floor(number);
};


const fromTo = function (start, end) {
  return Math.floor(Math.random() * (end - start)) + start;
};
```
---
## Fixing Syntax Errors
Common mistakes to watch for:

```js
// ❌ Incorrect
const myFunction = function parameter) {} // Missing '('
const my Second Function = function (parameter) {} // Invalid name
const function = function (parameter) {} // 'function' is a reserved keyword
const functionName = function (paramOne paramTwo) {} // Missing ','


// ✅ Correct
const myFunction = function (parameter) {};
const mySecondFunction = function (parameter) {};
const myFunctionName = function (paramOne, paramTwo) {};

```