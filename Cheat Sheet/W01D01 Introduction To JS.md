
# 📝W01D01 Introduction To JS

## 💡 What is JavaScript?
- **JavaScript**: A programming language used to add interactivity and dynamics to web pages.
- **Client-side**: Executed directly in the browser (Chrome, Firefox, Safari...).
- **Open the Console**:
  - Windows: `Ctrl + Shift + I` or `F12`
  - macOS: `Option + Command + I` or `F12`

---

## 🧠 Syntax
- Rules for writing correct code.
- Examples:
```js
1 + 1;
9 - 5;
3 * 4;
8 / 2;
```

---

## 🔢 Value Types

**Strings**
```js
"Hello", 'World'
"Hello" + " " + "World" // => "Hello World"
```

**Numbers**
```js
120, -56, 1.3, 0.8
10 % 3; // => 1
```

---

## 🔄 Mixing Types
```js
"I am " + 10 + " years old"; // => "I am 10 years old"
"10" - 5; // => 5
"10" + 1; // => "101"
```

---

## 📦 Variables

**Defining a Variable**
```js
const name = "Ali";
let age = 20;
age = 21;
```
Difference between `const` and `let`:
- `const`: Value cannot be reassigned.
- `let`: Value can be reassigned.
- `var`: Old and not recommended for modern usage.

---

## 🧾 Naming Rules

**✅ Allowed:**
```js
let myVar;
let $total;
let _counter;
let value123;
```

**❌ Not Allowed:**
```js
let 123name;
let var;
let const;
```
**Best Practice:** Use `camelCase` and meaningful names.

---

## 🧮 PEMDAS

P: Parentheses  
E: Exponents  
MD: Multiplication & Division (left to right)  
AS: Addition & Subtraction (left to right)

```js
9 + 1 * 5;           // => 14
(9 / 3) * (10 - 7);  // => 9
```

---

## 🧠 String Concatenation

```js
"John" + " " + "Doe" // => "John Doe"
```

---

## 🗨️ Comments

```js
// this is one line comment

/* Alt + Shift + A 
multi-line comment
*/
```

---

## 🔧 Writing a Program

The computer needs clear and specific instructions.  
Code runs top to bottom, left to right.

```js
console.log("Hello");
console.log(1 + 1);
```

---
### Practice Hints 

1. `let` variables can be reassigned; `const` variables cannot. Scope matters: variables declared inside a block (`{}`) are not accessible outside it.

2. Functions have their own local scope. Variables declared with `let` inside a function or block do not affect variables with the same name outside.

3. Use a **global variable** `counter` to store the current countdown value. Check if it’s greater than zero before decrementing, otherwise return a string.

4. Increment the same `counter` variable. Each invocation should increase its value by one.

5. Assign the passed `start` value to the `counter` variable. Return a string confirming the reset.

6. Create a global array or string to hold all items. Append the new item on each invocation and return the current list.

7. Use a **closure**: define the array or string inside `createToDoList` and return a function that modifies it. This keeps the data private to the closure.

8. Create a global variable `currentBalance`. Each deposit adds to this value and returns the updated balance.

9. Subtract the `amount` from `currentBalance`. If the amount is bigger than the balance, return a warning message.

10. Use a closure to store `balance`. Return a function that handles both `"deposit"` and `"withdraw"` actions, updating the balance accordingly. Prevent over-withdrawal.

11. Store maximum and minimum values in variables initialized to `Number.NEGATIVE_INFINITY` and `Number.POSITIVE_INFINITY`. Update them with each invocation and return a string with current max and min.

12. Maintain counters for wins and losses. Update them based on the game outcome, then return the score as a string.

13. Add a limit for the score. Once a player reaches the limit, reset the counters back to zero.

14. Introduce an optional boolean `reset` parameter. When `true`, reset the counters and return a reset message.

15. Track the last winner in a variable. Adjust the random move logic: if the user lost last round, give a 25% chance to repeat the previous move; otherwise, pick a random move.
