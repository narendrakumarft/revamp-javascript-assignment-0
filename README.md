# REVAMP ASSISGNMENT 0 - JavaScript Fundamentals Assignment

## 1. What is JavaScript?
- Provide a brief explanation of what JavaScript is and its role in web development.
```
JavaScript is the programming language of the web. 
It is also called as interpreted programming language, primarily used to create interactive and dynamic effects on websites. 
While most famous known for its role in front-end web development.
It can also be used for server-side development with platforms like Node.js
```

## 2. Variables and Types:
- Declare a variable named `userAge` and assign it a numerical value representing someone's age.
- Declare another variable named `userName` and assign it a string value representing a person's name.
- Output both variables using `console.log()`.
```javascript
let userAge = 30;
let userName = "Alice";

console.log(`${userName} is ${userAge} years old.`);
```

## 3. Comments in JavaScript:
- Write a multi-line comment explaining the purpose of a function you create in the next step.
```javascript
/*
 * Function: arithmetics(a, b)
 *
 * Purpose: This function serves as a utility to demonstrate the four
 * fundamental arithmetic operations (addition, subtraction, multiplication,
 * and division) between two numerical inputs, 'a' and 'b'.
 * It calculates all four results and prints them directly to the console
 * in a clearly formatted output.
 *
 * Parameters:
 * a - The first number.
 * b - The second number.
 *
 * Returns:
 * Logs the results of the four operations to the console.
 */
```

## 4. Operations:
- Create two variables, `num1` and `num2`, and assign them numerical values.
- Perform addition, subtraction, multiplication, and division operations on these variables.
- Display the results using `console.log()`.
```javascript
function arithmetics(a, b){
    let sum = a + b;
    let difference = a - b;
    let product = a * b;
    let quotient = a / b;

    console.log(`Arithmetic Results for ${a} and ${b}`);
    console.log(`Addition (${a} + ${b}):        `, sum);
    console.log(`Subtraction (${a} - ${b}):     `, difference);
    console.log(`Multiplication (${a} * ${b}):  `, product);
    console.log(`Division (${a} / ${b}):        `, quotient);
    console.log('-------------------------------------------');
}

let num1 = 28;
let num2 = 28;

arithmetics(num1, num2);
```

## 5. Data Types:
- Create variables to represent different data types: string, number, boolean, and an array.
- Provide examples and explain each data type.
```
1. A string is used to store text. String values are always enclosed in single quotes ('...'), double quotes ("..."), or backticks (`...`).
2. A number is used to store both integers (whole numbers) and floating-point numbers (decimals).
3. A boolean represents a logical entity and can only have one of two values: true or false.
4. An Array is a special type of object used to store an ordered list of values. These values can be of any data type (including other arrays or objects).
```
```javascript
let ex1 = "Hello, JavaScript!";
let ex2 = 28;
let ex3 = true;
let ex4 = false;
let ex5 = ["Apple", "Banana", "Carrot"];
let ex6 = ["Apple", "Banana", "Carrot", 28, true];

console.log("String Example:", ex1);
console.log("Type of above Example:", typeof ex1);
console.log("--------------------");
console.log("Number Example:", ex2);
console.log("Type of above Example:", typeof ex2);
console.log("--------------------");
console.log("Boolean Example:", ex3);
console.log("Type of above Example:", typeof ex3);
console.log("--------------------");
console.log("Boolean Example:", ex4);
console.log("Type of above Example:", typeof ex4);
console.log("--------------------");
console.log("Array Example:", ex5);
console.log("Type of above Example:", typeof ex5);
console.log("--------------------");
console.log("Object Example:", ex6);
console.log("Type of above Example:", typeof ex6);
```

## 6. Functions in JavaScript:
- Write a function named `greetUser` that takes a `name` parameter and returns a greeting message.
- Call the function with a sample name and display the result using `console.log()`.
```javascript
function greetUser(name){
    return `Hello, ${name}! Its Javascript Program is works!`;
}

let userName = "Narendrakumar";
let greetingMessage = greetUser(userName);

console.log(greetingMessage);
```

## 7. if Else in JavaScript:
- Create a variable named `temperature` and assign it a numerical value.
- Write an `if-else` statement to check if the temperature is greater than 30. Output a message accordingly
```javascript
let temperature = 28;

if(temperature > 30) {
    console.log(`${temperature}°C. It's hot outside!`);
} else {
    console.log(`${temperature}°C. It's a moderate day.`);
}
```

## 8. FOR LOOP:
- Use a `for` loop to print the numbers from 1 to 5 in the console.
```javascript
//A 'for' loop has three parts:
//1. Initialization (let i = 1): Starts the counter at 1.
//2. Condition (i <= 5): i is less than or equal to 5.
//3. Iteration (i++): Increases the counter by 1 after each cycle.
for (let i = 1; i <= 5; i++) {
    console.log(i);
}
```

## 9. Loose vs Strict Equality:
- Explain the difference between loose equality `(==)` and strict equality `(===)` with examples.
```
Loose Equality (==)
Performs type coercion: If the operands have different data types, == attempts to convert one or both operands to a common type before performing the comparison.
Returns true if the values are equal after potential type coercion.

Strict Equality (===)
Does not perform type coercion: === compares both the value and the data type of the operands.
Returns true only if both the value and the data type are identical.
```
```javascript
console.log(5 == "5");   // true (string "5" is coerced to number 5)
console.log(0 == false); // true (false is coerced to number 0)
console.log(null == undefined); // true (special case where they are considered loosely equal)

console.log(5 === "5");   // false (number 5 is not strictly equal to string "5")
console.log(0 === false); // false (number 0 is not strictly equal to boolean false)
console.log(null === undefined); // false (null and undefined are different types)
```

