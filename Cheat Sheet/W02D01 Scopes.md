
# W02D01 Scopes

## 📌 What is a Scope?

A **scope** is the context where variables and functions are accessible.
- It defines visibility.
- Helps manage variable lifecycle.

---

## 🌍 Global Scope

- Declared outside of any function/block.
- Accessible anywhere in the file.

```js
let name = "Alice";

function greet() {
  return name; // can access global variable
}
```

---

## 🧪 Local Scope

- Declared inside a function.
- Not accessible from the outside.

```js
function sayHi() {
  let greeting = "Hi";
  return greeting;
}

console.log(greeting); // ❌ ReferenceError
```

---

## 🔐 Block Scope

- Created using `{}` like in `if`, `for`, etc.
- `let` and `const` create block-scoped variables.

```js
if (true) {
  const age = 30;
}
console.log(age); // ❌ ReferenceError
```

- `var` is NOT block scoped.

```js
if (true) {
  var name = "John";
}
console.log(name); // ✅ "John"
```

---

## 🔁 Scope Chain

- Inner scope can access outer scope.
- Outer cannot access inner.

---

## 🔒 Closures

- A closure is a function that remembers its **lexical scope**, even after the outer function has finished executing.

```js
function counter() {
  let count = 0;
  return function () {
    return ++count;
  };
}

const count1 = counter();
count1(); // 1
count1(); // 2

const count2 = counter();
count2(); // 1
```

---

## 🧠 Summary

| Keyword | Scope Type  | Block Scoped | Hoisted |
|---------|-------------|--------------|---------|
| var     | Function    | ❌           | ✅       |
| let     | Block       | ✅           | ❌       |
| const   | Block       | ✅           | ❌       |

---

# 💡 Hints for Practices

## 🧪 Pulse Check

1. ✅ Declare `myFavoriteFood` **outside** the function.  
2. ✅ Reassign it from within a function using its name directly.  
3. ✅ Return a function from `createCounter_v01` and store it in a variable.  
4. ✅ Replace `let counter = 0` with `let counter = start`.

---

## 💼 Practice

1. 🔎 Watch how `let` and `const` behave differently in blocks.
2. 🔁 Inner `let` declarations don’t affect outer ones.
3. 📉 Use a global `counter = 5`, and check if it’s > 0 before decrementing.
4. 📈 Use same `counter` and increment it.
5. 🔄 Just reassign the global `counter = start` and return message.
6. 🧾 Declare `allList = ""` globally. Add `toDo` to it on each call.
7. 🧭 Use a closure variable `let list = ""` and return a function.
8. 💰 Declare `currentBalance = 0` globally. Add to it.
9. 🏦 Subtract from `currentBalance`, but only if enough funds.
10. 🔒 Inside closure, handle logic based on `transactionType`.

---

## 🧠 Advanced Practice

1. 📊 Use global `min = Infinity`, `max = -Infinity`, update them.
2. 🎮 Track wins/losses in global or closure variables.
3. 🎯 When win count reaches 5 (or 3), reset scores.
4. 🔁 Add optional param `reset` and check its value.
5. 🤖 If user loses, 25% chance the bot picks same move again.
