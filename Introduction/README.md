## 1. Comments & Outputting Data

JavaScript supports single-line and multi-line comments for documentation.

```javascript
// Single-line comment

/*
 Multi-line
 comment
*/

// Printing single and multiple values
console.log('Hello, World!');
console.log('JavaScript', 2026, true);
```
---

## 2. Basic Arithmetic Operations
JavaScript can perform standard mathematical evaluations directly:

```javascript
console.log(5 + 2);  // Addition (7)
console.log(5 - 2);  // Subtraction (3)
console.log(5 * 2);  // Multiplication (10)
console.log(5 / 2);  // Division (2.5)
console.log(5 % 2);  // Modulus / Remainder (1)
console.log(5 ** 2); // Exponentiation (25)
```
---
## 3. Data Types & Variables

JavaScript data types are divided into two main categories: 
**Primitive Data Types** (immutable) and 
**Non-Primitive Data Types** (mutable).

### Primitive Data Types

| Data Type | Description | Example |
| :--- | :--- | :--- |
| **String** | Text enclosed in single quotes, double quotes, or backticks | `'Hello'`, `"World"`, `` `JavaScript` `` |
| **Number** | Integers and floating-point decimal numbers | `25`, `-10`, `3.14` |
| **Boolean** | Logical entity representing `true` or `false` | `true`, `false` |
| **Undefined** | Declared variable without an assigned value | `let age;` |
| **Null** | Intentional absence of any object value | `let emptyVal = null;` |
| **Symbol** | Unique and immutable identifier | `Symbol('id')` |

### Non-Primitive Data Types (Arrays & Objects)

| Type | Syntax | Example | Access Values By |
| :--- | :--- | :--- | :--- |
| **Array** | `[ ]` (Square brackets) | `['apple', 'banana']` | Index number: `arr[0]` |
| **Object** | `{ }` (Curly braces) | `{ key: 'value' }` | Property name: `obj.key` |
---

### Checking Data Types (`typeof`)

Use the `typeof` operator to verify the data type of any variable or expression:

```javascript
console.log(typeof 'hello');      // "string"
console.log(typeof 250);         // "number"
console.log(typeof true);        // "boolean"
console.log(typeof undefined);   // "undefined"
console.log(typeof null);        // "object" (known JavaScript quirk)
```

### Declaring Variables (let vs const)
Variables store values in memory locations. Modern JavaScript uses let and const:

let: Used when values are expected to change over time.
const: Used for constants whose values will never change.
(Note: Avoid var due to scope hoisting issues).

<img width="955" height="470" alt="image" src="https://github.com/user-attachments/assets/30d4020e-08da-42e0-8c75-e0531e56c94d" />


```javascript
// Mutable variable
let currentAge = 25;
currentAge = 26; // Reassignment allowed

// Immutable constant
const GRAVITY = 9.81;
const PI = 3.14;
```

### Variable Naming Rules & Conventions
A valid JavaScript variable name must follow these rules:

1. **No Starting Numbers**: A variable name cannot begin with a digit (e.g., `1number` is invalid, but `number1` is valid).
2. **Allowed Characters**: Letters, numbers, dollar signs (`$`), and underscores (`_`) are allowed. Other special characters (like `-`, `@`, `#`, `%`) are strictly prohibited.
3. **No Spaces**: Variable names cannot contain spaces (e.g., `first Name` is invalid).
4. **camelCase Convention**: Multi-word variable names standardly use camelCase (e.g., `firstName`, `isLoggedIn`, `totalItemCount`).

---

## 4. Adding JavaScript to a Web Page

JavaScript can be added to an HTML document in three different ways:

### 1. Inline Script
Inline scripts are written directly inside HTML attributes (such as `onclick`).

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Inline Script</title>
  </head>
  <body>
    <button onclick="alert('Hello, World!')">Click Me</button>
  </body>
</html>
// Declaring multiple variables
let firstName = 'Asabeneh',
    job = 'Teacher',
    isMarried = true;
```
### 2. Internal Script
Internal scripts are written inside <script> tags within the HTML file. While they can be placed in <head>, placing them before the closing </body> tag is preferred for faster page loading.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Internal Script</title>
  </head>
  <body>
    <button onclick="alert('Hello, World!')">Click Me</button>

    <script>
      console.log('Hello, World!');
    </script>
  </body>
</html>
```

### 3. External & Multiple External Scripts
External scripts keep code modular and clean by linking standalone .js files using the src attribute.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Multiple External Scripts</title>
  </head>
  <body>
    <!-- Link external JS files before the closing body tag -->
    <script src="./helloworld.js"></script>
    <script src="./introduction.js"></script>
  </body>
</html>
```
