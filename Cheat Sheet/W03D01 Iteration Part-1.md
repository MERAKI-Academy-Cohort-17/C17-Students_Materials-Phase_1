
# 🔁 JavaScript Iteration Cheat Sheet

## 🎯 Learning Goals

- Use `while` and `for` loops
- Iterate over arrays and strings
- Avoid common loop mistakes

---

## 🌀 While Loops

A `while` loop runs **as long as the condition is true**.

```js
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

💡 You control:
- Start: `let i = 0`
- Condition: `i < 5`
- Step: `i++`

✅ You can also use non-numeric conditions:

```js
let found = false;
while (!found) {
  // do something
}
```

---

## 🔁 For Loops

Used when the number of iterations is known.

```js
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

### Multiple variables in for loop:

```js
for (let i = 0, j = 10; i < j; i++, j--) {
  console.log(i, j);
}
```

### Break & Continue

```js
for (let i = 0; true; i++) {
  if (i === 3) continue;
  if (i === 5) break;
  console.log(i);
}
```

---

## 🧱 Iterating Arrays

Arrays are indexed => start from `0` to `array.length - 1`

```js
const arr = [1, -2, 3];
for (let i = 0; i < arr.length; i++) {
  if (arr[i] >= 0) console.log(arr[i]);
}
```

---

## 🔤 Iterating Strings

Strings work like arrays: indexed characters

```js
const str = "John";
for (let i = 0; i < str.length; i++) {
  console.log(str[i]);
}
```

---

## ⚠️ Common Mistakes

### ❌ Wrong condition
```js
let i = 0;
while (i < -10) { ... } // never runs
```

### ❌ Infinite loop
```js
let i = 0;
while (i < 10) {
  console.log(i);
  i--; // goes the wrong way!
}
```

### ❌ Reusing modified index
```js
let i = 0;
while (i < 5) {
  i++;
}
while (i < 5) { // will not run
  i++;
}
```

---

## 🧯 Infinite Loop Fixes

- Browser tab frozen? Close tab or force-quit browser.
- Windows: Task Manager `CTRL + SHIFT + ESC`
- macOS: Activity Monitor `CMD + OPTION + ESC` or search

---

## ✅ Summary Table

| Concept           | Key Idea                                |
|-------------------|------------------------------------------|
| `while` loop      | Run while condition is true              |
| `for` loop        | Known number of steps                    |
| `break`           | Stop loop immediately                    |
| `continue`        | Skip current iteration                   |
| Arrays/Strings    | Both are index-based, use `.length`      |
| Loop Errors       | Watch condition, step, and reuse of vars |


---


# JavaScript Practice Hints

---

1. 🔹 **Fixing loops**  
   - Use `let` or `var` for loop variables, not `const`.  
   - Make sure your loop condition makes sense (`i < 10`) and the increment/decrement is correct (`i++` or `i--`).

2. 🔹 **While loop from 0 to 5**  
   - Start from 0 and loop while `<= 5`.  
   - Increment your counter inside the loop to avoid infinite loops.

3. 🔹 **For loop from 10 to 20**  
   - Use `for (let i = 10; i <= 20; i++)` to include start and end numbers.

4. 🔹 **Array loop with index and value**  
   - Loop through the array with `i = 0; i < array.length; i++`.  
   - Access values with `array[i]` and keep track of the index with `i`.

5. 🔹 **String loop skipping 'a'**  
   - Loop through each character.  
   - Use `if (string[i] !== 'a')` to skip unwanted letters.

---

## Practice

6. 🔹 **Sum function**  
   - Start with `let total = 0`.  
   - Loop through each number and add it to `total`.

7. 🔹 **Login function**  
   - Check each user object for both `username` and `password`.  
   - Return success if matched, otherwise failure.

8. 🔹 **Filter strings**  
   - Use `typeof element === "string"` to keep only strings.

9. 🔹 **Range function**  
   - If only one number is provided, treat the other as 0.  
   - Ensure numbers are ascending, even if start > end.  
   - Include both start and end.

10. 🔹 **Only odd numbers**  
    - Use `number % 2 !== 0` to detect odd numbers.

11. 🔹 **Maximum number**  
    - Start with the first number as a reference.  
    - Compare and update the maximum as you loop.

12. 🔹 **Reverse string**  
    - Start with an empty string.  
    - Add characters from the end to the beginning.

13. 🔹 **Only even numbers (same array)**  
    - Use `splice()` to remove numbers that are not even.  
    - Adjust the index carefully after removing elements.

14. 🔹 **Create user**  
    - Check if the username already exists.  
    - Return rejection if taken, otherwise add user and return success.

15. 🔹 **Convert array to object**  
    - Loop through the array.  
    - Assign `obj[index] = value`.

