Node.js Custom Module Assignment
1. Create a `greetings.js` Module
Code:
```js
// greetings.js
function greet(name) {
return `Hello, ${name}! Welcome to the Node.js module system.`;
}
module.exports = greet;
```
2. Create a `mathOperations.js` Module
Code:
```js
// mathOperations.js
function add(a, b) {
return a + b;
}
function subtract(a, b) {
return a - b;
}
function multiply(a, b) {
return a * b;
}
function divide(a, b) {
return a / b;
}
module.exports = { add, subtract, multiply, divide };
```
3. Create a `main.js` File
Code:
```js
// main.js
const greet = require('./greetings');
const math = require('./mathOperations');
const name = 'Alice';
console.log(greet(name));
console.log("Addition: ", math.add(10, 5));
console.log("Subtraction: ", math.subtract(10, 5));
console.log("Multiplication: ", math.multiply(10, 5));
console.log("Division: ", math.divide(10, 5));
```
