
# JavaScript Control Structures

Control structures determine the execution flow of your JavaScript code based on conditions and loops.

---

## 1. Conditional Statements

Conditional statements execute specific code blocks only when given conditions evaluate to `true`.

### `if`, `else if`, and `else`
Evaluates conditions sequentially from top to bottom.

```javascript
let score = 85;

if (score >= 90) {
  console.log('Grade: A');
} else if (score >= 80) {
  console.log('Grade: B'); // Output: Grade: B
} else if (score >= 70) {
  console.log('Grade: C');
} else {
  console.log('Grade: F');
}
```

### switch Statement
Ideal when matching a single variable against multiple discrete values.

```javascript
let day = 'Monday';

switch (day) {
  case 'Monday':
    console.log('Start of the work week.');
    break; // Exits the switch block
  case 'Friday':
    console.log('Weekend is near!');
    break;
  default:
    console.log('Just another day.');
}
```


## 2. Iteration & Loops
Loops repeat a block of code until a specified condition becomes false.

## A. for Loop
Used when the number of iterations is known in advance.
```javascript
// Syntax: for (initialization; condition; increment/decrement)
for (let i = 0; i < 3; i++) {
  console.log(`Iteration ${i}`);
}
// Output:
// Iteration 0
// Iteration 1
// Iteration 2
```

## B. while Loop
Executes as long as the specified condition remains true.
```javascript
let count = 0;

while (count < 3) {
  console.log(`Count is: ${count}`);
  count++;
}
```

## C. do...while Loop
Guarantees the code block runs at least once before evaluating the condition.
```javascript
let number = 5;

do {
  console.log(`Number is: ${number}`); // Runs once even if condition is false
  number++;
} while (number < 3);
```
```

