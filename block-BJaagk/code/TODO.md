Convert the function below into different forms of function expression.
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage = function (marks, total) {
  return (marks * 100) / 100;
}

let percentage =  (marks, total) => {
  return (marks * 100) / 100;
}


Write Function Declaration or Function Expression next to the function.
function percentage(marks, total) {
  return (marks * 100) / total;
}

// declaration
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

// function expression
let percentage = function (marks, total) {
  return (marks * 100) / total;
};

// function expression
//

let percentage = (marks, total) => {
  return (marks * 100) / total;
};

// function expression
let percentage = (marks, total) => (marks * 100) / total;
// function expression
Why is a function definition an expression in JavaScript? Give one example of function expression. function is object and oject is value
function add(){

}

var obj = {};
let add  = function(){}
Why is a function call an expression in JavaScript?

Write VALID and INVALID next to each example below with the reason.

function add(a, b) {
  return a + b;
}

let five = add(2, 3); // valid because function is a object and object is store in a variable that type function is call function expression
five = add; // vaild because add is function refrence 
five = five(10, 11); // vaild it is function expression 
five = function () {
  return 'Hello';
}; // Answer  VALID function is a object and object is expression variable can store expression 
What is the difference between function definition and function call? Explain with an example.
// function definition
function name() {
  return "ravindra"
}


// function call 
name()
What is the similarities between function definition and function call?
function name is same when we will define function and call the function

Is the code below valid or invalid. Explain with reason.
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid function is a object 
What is higher order function explain with an example.
when a function that accepts function definition as an argument is know as heigher order function

function sum(add){
  return add(2,5);
}

sum(function add(a,b)  {
  return a + b;
})

Explain what is callback function. Why you can pass a function inside a function?
when a function pass as a argument that type function is called call back function.

we pass function refrence inside the function because function is a object and object is expression.