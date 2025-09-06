 Day 1 - 2025-09-07
# Topic: Hoisting

+ Definition
Hoisting is the process in JavaScript where **variable declarations (`var`)** and **function declarations** are moved to the top of their scope (memory is allocated) before the code executes.

+ Key Points
- `var` → declaration is hoisted, but value is not assigned. Default value = `undefined`.
- `let` / `const` → are also hoisted, but they stay in **Temporal Dead Zone (TDZ)** until initialized. Accessing them before initialization throws an error.
- Function declarations → fully hoisted, so they can be called before being defined.

---

# Example 
```js
console.log(a); // undefined
var a = 5;
console.log(a); // 5

+Internally JavaScript treats it like this:
var a;              // declaration hoisted
console.log(a);     // undefined
a = 5;              // assignment
console.log(a);     // 5

# Function Hoisting
sayHello(); 

function sayHello() {
  console.log("Hello World!");
}


