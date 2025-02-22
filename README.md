# Js-callback
# Callbacks in JavaScript

In JavaScript, a **callback** is a function that is passed as an argument to another function and is executed after the other function has finished executing. Callbacks are commonly used to handle asynchronous operations such as reading files, handling events, or working with APIs.

## Simple Callback Example

A basic example of how callbacks work:

```javascript
function greet(name, callback) {
  console.log("Hello " + name);
  callback(); // Call the callback function
}

function afterGreet() {
  console.log("Greeting complete!");
}

greet("John", afterGreet);
