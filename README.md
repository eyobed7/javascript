
# JavaScript for Absolute Beginners

Welcome to your beginner guide to JavaScript. Each "slide" is a topic. Use the outline below to navigate.

---

## 🧭 Outline

1. [Console and `console.log()`](#1-console-and-consolelog)
2. [Variables](#2-variables)
3. [Data Types: Number](#3-data-types-number)
4. [Data Types: String](#4-data-types-string)
5. [Math Operators](#5-math-operators)
6. [Operator Precedence (BIDMAS)](#6-operator-precedence-bidmas)
7. [Shorthand Operators](#7-shorthand-operators)
8. [NaN](#8-nan)
9. [String Interpolation (Backticks)](#9-string-interpolation-backticks)
10. [Undefined](#10-undefined)
11. [Null](#11-null)
12. [Arrays](#12-arrays)
13. [Boolean](#  boolean)
14. [Control Flow (Loops)](# Control flow)

---

## 1. Console and `console.log()`

- The **console** is a tool to test and debug JavaScript.
- `console.log()` prints messages to the browser console.

```javascript
console.log("Hello, JavaScript beginner!"); // This will show the message in the console
```

---

## 2. Variables

- Variables store data. Think of them like containers.

```javascript
let name = "Eyobed"; // using let
const pi = 3.14; // using const for values that don't change
var age = 25; // older way, not recommended now
```

---

## 3. Data Types: Number

- Numbers can be integers or decimals.

```javascript
let score = 100;
let price = 19.99;

console.log(score + price); // 119.99
```

---

## 4. Data Types: String

- Strings are text wrapped in quotes.

```javascript
let firstName = "Eyobed";
let lastName = "Sebrala";

// Concatenation with +
let fullName = firstName + " " + lastName;
console.log(fullName); // Eyobed Sebrala

// Getting character by index
console.log(fullName[0]); // E

// Properties
console.log(fullName.length); // 15

// Methods
console.log(fullName.toUpperCase()); // EYOBED SEBRALA
console.log(fullName.toLowerCase()); // eyobed sebrala
console.log(fullName.indexOf("e")); // returns first index of 'e'
console.log(fullName.lastIndexOf("e")); // returns last index of 'e'
console.log(fullName.slice(0, 6)); // Eyobed
console.log(fullName.substr(7, 7)); // Sebrala
console.log(fullName.replace("Eyobed", "Eyo")); // Eyo Sebrala
```

---

## 5. Math Operators

- Used for calculations: `+`, `-`, `*`, `/`, `%`, `**`

```javascript
let radius = 7;
const pi = 3.14159;
let area = pi * radius ** 2; // Area of a circle
console.log(area); // 153.938

let a = 10;
let b = 3;
console.log(a % b); // 1 (remainder)
```

---

## 6. Operator Precedence (BIDMAS)

- **BIDMAS**: Brackets, Indices, Division/Multiplication, Addition/Subtraction

```javascript
let result = 2 + 3 * 4; // 2 + 12 = 14
let correct = (2 + 3) * 4; // 5 * 4 = 20
console.log(result);
console.log(correct);
```

---

## 7. Shorthand Operators

```javascript
let count = 5;
count++; // increases by 1
count--; // decreases by 1

count += 3; // adds 3
count -= 2; // subtracts 2
count *= 2; // multiplies by 2
count /= 2; // divides by 2

console.log(count); // check final value
```

---

## 8. NaN

- **NaN** stands for “Not a Number”

```javascript
let result = 100 / "Eyobed";
console.log(result); // NaN
```

---

## 9. String Interpolation (Backticks)

- Use backticks `` ` `` and `${}` to embed variables in strings

```javascript
let name = "Eyobed";
let age = 25;
let message = `Hello, my name is ${name} and I am ${age} years old.`;
console.log(message);
```

---

## 10. Undefined

- A variable declared but not given a value is `undefined`.

```javascript
let test;
console.log(test); // undefined
```

---

## 11. Null

- `null` is an intentional empty value.

```javascript
let data = null;
console.log(data); // null
```

---

## 12. Arrays

- Arrays store multiple values in one variable.

```javascript
let colors = ["red", "green", "blue"];

console.log(colors[0]); // red
console.log(colors.length); // 3

// Methods
console.log(colors.join(" - ")); // "red - green - blue"

let moreColors = ["yellow", "purple"];
let allColors = colors.concat(moreColors);
console.log(allColors); // merges arrays

colors.push("black"); // adds to end
console.log(colors); 

colors.pop(); // removes last element
console.log(colors); 

console.log(colors.indexOf("green")); // 1
```

---

Thanks for reading! You can now write and debug JavaScript like a pro beginner! 🎉


---

## 13. Boolean Data Type

- Booleans represent **true** or **false** values.

```javascript
let isOnline = true;
let hasAccess = false;

console.log(typeof isOnline); // boolean
console.log(5 > 3); // true
console.log(10 === "10"); // false (different types)
```

---

## 14. Control Flow (Loops)

- Control flow means the order in which the code runs.
- Loops let you repeat tasks.

### `for` Loop

```javascript
// Print numbers 1 to 5
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

### `while` Loop

```javascript
let count = 1;
while (count <= 5) {
  console.log(count);
  count++;
}
```

### `do...while` Loop

```javascript
let num = 1;
do {
  console.log(num);
  num++;
} while (num <= 5);
```

- `do...while` runs **at least once**, even if the condition is false.

---

## 15. Conditional Statements (`if`, `else`, `else if`)

- They let you run code only when certain conditions are met.

```javascript
let score = 85;

if (score >= 90) {
  console.log("Excellent!");
} else if (score >= 75) {
  console.log("Very Good!");
} else {
  console.log("Keep trying!");
}
```

---

## 16. Logical Operators

- Used to combine conditions.

| Operator | Description       | Example                  | Result         |
|----------|-------------------|--------------------------|----------------|
| `&&`     | AND (both true)   | `true && false`          | false          |
| `||`     | OR (at least one) | `true || false`          | true           |
| `!`      | NOT (opposite)    | `!true`                  | false          |

```javascript
let age = 20;
let hasTicket = true;

if (age >= 18 && hasTicket) {
  console.log("You can enter.");
}

if (age < 18 || !hasTicket) {
  console.log("Entry denied.");
}
```

---
