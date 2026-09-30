# JavaScript Functions

Functions are reusable blocks of code designed to perform a specific task. They keep your code modular, readable, and DRY (Don't Repeat Yourself).

---

## 1. Function Declarations vs. Expressions

### A. Function Declaration
Declared using the `function` keyword. Declarations are **hoisted**, meaning they can be called before they appear in the code.

```javascript
// Function Declaration
function greet(name) {
  return `Hello, ${name}!`;
}

console.log(greet('Alex')); // Output: Hello, Alex!
```

### B. Function Expression
A function assigned to a variable. Expressions are not hoisted, so they must be defined before they are called.

```JavaScript
// Function Expression
const speak = function(name) {
  return `Welcome, ${name}!`;
};

console.log(speak('Sam')); // Output: Welcome, Sam!
```

## 2. Arrow Functions (ES6)
Arrow functions provide a shorter syntax and do not have their own this context.

```JavaScript
// Standard Arrow Function
const multiply = (a, b) => {
  return a * b;
};

// Implicit Return (One-liner syntax)
const add = (a, b) => a + b;
const square = n => n * n; // Parentheses optional for a single parameter

console.log(add(5, 3));    // Output: 8
console.log(square(4));   // Output: 16
```

## 3. Parameters & Arguments
Parameters: Variable names listed in the function definition.

Arguments: Real values passed to the function when it is invoked.

### A. Default Parameters
Provide fallback values if no argument is passed during execution.

```JavaScript
function welcomeUser(name = 'Guest') {
  return `Hello, ${name}!`;
}

console.log(welcomeUser());        // Output: Hello, Guest!
console.log(welcomeUser('Taylor')); // Output: Hello, Taylor!
```

### B. Rest Parameters (...)
Gathers multiple arguments into a single array array variable.

```JavaScript
function sumAll(...numbers) {
  return numbers.reduce((total, num) => total + num, 0);
}

console.log(sumAll(1, 2, 3, 4)); // Output: 10
```

## 4. Higher-Order & Callback Functions
Callback Function: A function passed as an argument to another function.

Higher-Order Function: A function that takes another function as an argument or returns a function.

```
JavaScript
// Callback function
const printResult = (result) => console.log(`The result is: ${result}`);

// Higher-order function
function calculate(num1, num2, callback) {
  const sum = num1 + num2;
  callback(sum);
```
}

calculate(10, 20, printResult); // Output: The result is: 30
