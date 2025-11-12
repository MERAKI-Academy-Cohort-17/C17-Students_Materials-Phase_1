# JavaScript Basics Cheat Sheet


## 🧠 Booleans

Represents true or false.

Can also behave like numbers:

- true → 1

- false → 0

## Comparison Operators

Used to compare values, result is always true or false.

### Operator	Meaning
>	Greater than
<	Less than
>=	Greater than or equal
<=	Less than or equal
===	Strictly equal (value + type)
!==	Strictly not equal
==	Loosely equal (not recommended)
🔗 Logical Operators

Used to combine conditions:

Operator	Name	Description
&&	AND	Both must be true → true
`		`
!	NOT	Reverses the value
### 🧾 Conditional Statements

Run different code based on conditions.

if → Runs code if condition is true.

else → Runs if all above conditions are false.

else if → Allows multiple conditions.

### 🗝️ Truthy & Falsy Values

Falsy Values: 0, undefined, null, "", false, NaN.

Everything else is truthy.

#### Example:

if ("hello") → Runs (truthy)

if (0) → Skipped (falsy)

## 🧮 Practice Hints

1. Understanding Comparison Errors

- Double-check operator symbols and condition structure.

- Ensure parentheses are placed correctly.

2. Predicting Boolean Expressions

- Break them down step by step.

- Evaluate && before ||.

- Remember ! reverses the value.

3. Function Logic Tips

- Use if and else to handle different cases.

- Think about edge cases like exact boundaries.

- Check the type of the input before processing.

- Pay attention to string length and case sensitivity.

- Keep conditions organized and readable.

4. Strings & Characters

- You can access specific letters using index positions.

- Consider case-insensitive checks by converting strings first.

5. Numbers & Calculations

- Use modulo % for checking even/odd.

- Validate numbers to prevent unexpected behavior.

6. Login Logic

- Check username and password lengths first.

- Compare username case-insensitively but password exactly.

- Return clear feedback for each type of failure.

### 💡 Extra Tip

Start with clear conditions before adding complexity.

Keep testing small parts to confirm your logic works correctly.
