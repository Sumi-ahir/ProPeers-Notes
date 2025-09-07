### 🚀 Topic: JavaScript Arrow Function `this`

####  Question
What will be logged to the console?

```javascript
const proPeersFunc = () => {
  console.log(this === window);
};
proPeersFunc();

✅ Answer
TRUE

📝 Explanation

Arrow functions (()=>) lexical this binding use કરે છે, એટલે arrow function પોતાનું this નથી બનાવતું.

Global scope માં, this browser environment માં window ને refer કરે છે.

Arrow function upper scope ના this (global scope) ને use કરે છે.

તેથી this === window evaluate થાય છે અને console માં TRUE log થાય છે.
