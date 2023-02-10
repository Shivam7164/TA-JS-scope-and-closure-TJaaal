Find the output of the code snippets below:

console.log(numA + numB); // NaN
var numA = 21,
  numB = 30;

Find the output of the code snippets below:

console.log(numA + numB); // NumA is not defined
let numA = 21,
  numB = 30;



Find the output of the code snippets below:

let numA = 21,
  numB = 30;
console.log(numA + numB); // 51



Find the output of the code snippets below:

console.log(sayHello()); // 'hello'
function sayHello() {
  console.log("Hey");
}
function sayHello() {
  console.log("Hello");
}


Find the output of the code snippets below:

let username = "Tyrion";
sayHello(); // 'tyrion'
function sayHello() {
  console.log(username);
}



Find the output of the code snippets below:

sayHello(); // user name is not defined
let username = "Tyrion";
function sayHello() {
  console.log(username);
}



Find the output of the code snippets below:

let username = "Tyrion";
sayHello(); // sayHello is not defined
let sayHello = () => {
  console.log(username);
};


Find the output of the code snippets below:

sayHello(); // sayHello is not defined
let username = "Tyrion";
let sayHello = () => {
  console.log(username);
};



Find the output of the code snippets below:

sayHello(); // sayHello is not defined
var username = "Tyrion";
let sayHello = () => {
  console.log(username);
};


Find the output of the code snippets below:

var username = "Tyrion";
sayHello(); //  sayHello is not defined
let sayHello = () => {
  console.log(username);
};


Find the output of the code snippets below:

var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  var username = "John";
};
sayHello(); // undefined
Find the output of the code snippets below:

var username = "Tyrion";
let sayHello = () => {
  var username = "John";
  console.log(username);
};
sayHello(); // "John"

Find the output of the code snippets below:

var username = "Tyrion";
let sayHello = () => {
  console.log(username);
  let username = "John";
};
sayHello(); // referenceError cannot access "username"