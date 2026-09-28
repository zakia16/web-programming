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

## 3. Data Types & Variables

JavaScript data types are divided into two main categories: **Primitive Data Types** (immutable) and **Non-Primitive Data Types** (mutable).

### Primitive Data Types

| Data Type | Description | Example |
| :--- | :--- | :--- |
| **String** | Text enclosed in single quotes, double quotes, or backticks | `'Hello'`, `"World"`, `` `JavaScript` `` |
| **Number** | Integers and floating-point decimal numbers | `25`, `-10`, `3.14` |
| **Boolean** | Logical entity representing `true` or `false` | `true`, `false` |
| **Undefined** | Declared variable without an assigned value | `let age;` |
| **Null** | Intentional absence of any object value | `let emptyVal = null;` |
| **Symbol** | Unique and immutable identifier | `Symbol('id')` |

---

### Checking Data Types (`typeof`)

Use the `typeof` operator to verify the data type of any variable or expression:

```javascript
console.log(typeof 'Asabeneh'); // "string"
console.log(typeof 250);         // "number"
console.log(typeof true);        // "boolean"
console.log(typeof undefined);   // "undefined"
console.log(typeof null);        // "object" (known JavaScript quirk)
