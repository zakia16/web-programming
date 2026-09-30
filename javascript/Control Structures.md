
# JavaScript Control Structures

Control structures determine the execution flow of your JavaScript code based on conditions and loops.

---

## 1. Conditional Statements

Conditional statements execute specific code blocks only when given conditions evaluate to `true`.

### A. `if`, `else if`, and `else`
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
