# 📝W02D03- Arrays In JavaScript Cheat Sheet
## What Are Arrays?
- Ordered collections of values.


- Can hold any data type.
```js
const empty = [];
const fruits = ["Apple", "Banana"];
const mixed = [42, "Hi", true, [1, 2], function() {}];
```
---

## Accessing Array Values
Index starts at 0.
```js
const nums = [10, 20, 30];
nums[0];           // => 10
nums[nums.length - 1]; // => 30
```
---


## Nested arrays:
```js
const nested = [[1, 2], [3, 4]];
nested[1][0]; // => 3
```
---
## Assigning Values 
```js
let arr = [1, 2, 3];
arr[0] = 9;   // [9, 2, 3]
arr[3] = 4;   // [9, 2, 3, 4]
```
---







 ## Array Properties & Methods


| Method         | Description             | Example         |
|----------------|-------------------------|------------------|
| `.length`      | Returns number of elements | `arr.length`     |
| `.push(val)`   | Adds to end             | `arr.push(5)`     |
| `.pop()`       | Removes last item       | `arr.pop()`       |
| `.unshift(val)`| Adds to start           | `arr.unshift(0)`  |
| `.shift()`     | Removes first item      | `arr.shift()`     |
| `.join(sep)`   | Combines into string    | `arr.join("-")`   |
| `.reverse()`   | Reverses the array      | `arr.reverse()`   |
  
### Examples
```js

// ✅ Add Element to End of Array
const arr = [1, 2, 3];
arr.push("New"); // arr is now [1, 2, 3, "New"]


// ✅ Add Element to Start of Array
arr.unshift("First"); // arr is now ["First", 1, 2, 3, "New"]


// ✅ Create a String from Array Elements
const words = ["Hi", "there"];
const sentence = words.join(" "); // => "Hi there"


// ✅ Reverse an Array
const reversed = [1, 2, 3].reverse(); // => [3, 2, 1]

```
---

