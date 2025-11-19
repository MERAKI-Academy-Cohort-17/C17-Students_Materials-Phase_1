# 📝 W01D03 Objects in JavaScript

## 🧱 Objects

- Objects are collections of key-value pairs.

- Keys are like labels, values can be any type (number, string, array, boolean, another object, or even a function).

- Used to group related information together.

## ✏️ Defining an Object

- Use {} to create objects.

- Keys and values are separated by : and each pair is separated by ,.

- You can store different types of data in one object.

- You can also use variables as values inside objects.

## 🔍 Accessing Values

There are two ways to access values in an object:


| Method               | Example         | When to Use                          |
| -------------------- | --------------- | ------------------------------------ |
| **Dot Notation**     | `object.key`    | When you know the key name directly  |
| **Bracket Notation** | `object["key"]` | When the key is stored in a variable |

##### `Bracket notation works with variables, dot notation does not.`

## ✏️ Assigning / Updating Values

- You can add new keys or update existing ones using the assignment operator =.

- Works with both dot notation and bracket notation.

#### Example thought process:

- Add a new key → "Attach" a new piece of data to the object.

- Update a key → Replace the old value with a new one.

## 🏭 Factory Functions

- A factory function is a regular function that creates and returns objects.

- Useful when you need to create many similar objects without repeating code.

- Think of it as a template for making objects.

## 🧮 Practice Hints

1. Defining Objects

- Group related data under clear, descriptive keys.

- Nested objects can be used for more structured data.

2. Accessing Data

- Use dot notation for direct access.

- Use bracket notation when working with dynamic keys or variables.

- For nested data, chain notations step by step.

3. Updating and Adding Properties

- Double-check if you're updating an existing property or adding a new one.

- Remember, missing keys will automatically be created when assigned.

4. Finding Syntax Errors

- Watch for:

   - Missing , between key-value pairs.

   - Using : instead of = incorrectly.

   - Missing {} or quotes for strings.

5. Nested Objects & Arrays

- Access data step-by-step, one level at a time.

- Use the correct combination of [] for arrays and . or [] for objects.

6. Working with Lists of Objects

- Loop through them if needed.

- Always specify which object or index you're trying to reach.

7. Factory Functions

- Clearly define what data you need to create.

- Return a new object each time the function runs.

8. Counting and Checking Keys

- There are built-in tools to list all keys and count them.

- Also ways to check if a key exists before using it.

9. Transforming Values

- You can extract all values and combine them into a single string or other formats.

- Think step-by-step: first get the values, then process them.

10. Validation

- Check data before using it:

   - Is it a number?

   - Does the key exist?

   - Is the value in the correct format?

### 💡 Extra Tip

- Objects are everywhere in JavaScript (even arrays and functions are special kinds of objects).

- Always think of objects as a container for related information.

- Start simple, then add complexity step by step.
