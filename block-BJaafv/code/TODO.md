1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
The difference between the two sum functions is that the first function is using return keyword to return a value while the 2nd function is logging the value in console by using console.log.


2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
   
   If we pass arguments such as sum(2,2); for the first function the variable first will store the value for the operation and return 4.
   The variable second will also store the value of the operation performed in the console.log(a+b); which will be 4.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

   The output will be 36 as it will take only two arguments.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
   
   Yes, functions in JavaScript can be stored in a variable , because they act as a value and values can be stored. Functions are objects in JavaScript and Objects are values and also expressions. Below is an example of Function expression.
   ```js
    let add= function sum(a, b) {
  return a + b;
}```
5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
  ```js
   sayHello(name){
     return 'Hello' +' '+ name;
   }
   sayHello(Arya);
   ```

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();   
```
  //Output "Hello, John", The variable userName is defined as a global variable so it can be used in the function. 

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1   userName 'John' will be alerted.

showMessage(); // Output 2      'Hello, John'

alert(userName); // Output 3   userName 'John' will be alerted.
```

8. What is a Anonymous Function give example of three functions.

    Anonymous functions are functions without name and they can be called by their variable name.
    for example: const add= function(a,b){ return a+b;};
                 const sub= funciton(c,d){ return c-d;};
                 const mul=function(e,f){return e*f;}; 
                 
9. Can function declaration be a Anonymous Function? Explain
   
   function declaration cannot be Anonymous as it has the name of the function.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
```js
// example 1: a function to add 2 numbers.
  function addNumbers(numA,numB){
    return numA+numB;
  } 
//example 2: a function to alert Hello World.
function displaymsg(msg){
    alert("Hello World");
}
//example 3: a function to calculate area of rectangle
function calcArea(l,b){
  return l*b;
}
// example 4: a funciton to check for even numbers
function checkEven(n){
  if(n%2===0){
    return `Number is even`;
  }
  else{
    return `Number is not even`;
  }
}
// example 5: a function to get the factorial of number.
 
 function getFactorial(num){
    if(num==0||num==1){
      return 1;
    }
    else{
      return num * getFactorial(num-1);
    }
   
 }