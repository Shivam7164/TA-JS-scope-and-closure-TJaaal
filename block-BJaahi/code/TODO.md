For the given code below:

re-write the code in ways that system will understand
For Example:

1.  var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');

// Your code goes here
//Declaration phase

var username = undefined
let brother;

function sayHello(name) {
  return `Hello ${name}`;
}
let message;
var nextMessage;

//Execution phase

 username = 'Arya';
 brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);
 message = sayHello(username);
nextMessage = sayHello('Test');



2. 
console.log(username, numbers);
var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');

// Your code goes here
//Declaration phase

var username = undefined;
let number;
function sayHello(name) {
  return `Hello ${name}`;
}
let message;
var nextMessage = undefined

//Execution phase

console.log(username, numbers);
username = 'Arya';
number = 21;
message = sayHello(username);
nextMessage = sayHello('Test');

3. 
console.log(username, numbers);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');

// Your code goes here

//Declaration phase
let username;
let number;
let sayHello = function (name) {
  return `Hello ${name}`;
};
let message;
var nextMessage = undefined

//Execution phase

console.log(username, numbers);
username = 'Arya';
number = 21;
message = sayHello(username);
nextMessage = sayHello('Test');

4. let username = 'Arya';
console.log(username, numbers);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = sayHello('Test');

// Your code goes here
//Declaration phase
let username;
let number;
let message;
let sayHello = function (name) {
  return `Hello ${name}`;
};
var nextMessage = undefined


//Execution phase

username = 'Arya';
console.log(username, numbers);
number = 21;
message = sayHello(username)
nextMessage = sayHello('Test');

5. 
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;

// Your code goes here
//Declaration phase

var name = undefined
let age;

//Execution phase
console.log(name);
console.log(age);
name = 'Lydia';
age = 21;

6. function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();

// Your code goes here
//Declaration phase

function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

//Execution phase

sayHi()

7. sayHi();
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

// Your code goes here
//Declaration phase
sayHi();
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

//Execution phase
sayHi()


8. sayHi();
let sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};

// Your code goes here
//Declaration phase
let sayHi;

//Execution phase
sayHi()

9. let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;

// Your code goes here
//Declaration phase
let num1;
var sum = undefined
let num2;


//Execution phase
console.log(sum);
sum = num1 + num2
num2 = 30;

10. var num1 = 21;
let sum2 = addAgain(num1, num2, 4, 5, 6);
let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);

// Your code goes here
//Declaration phase

var num1 = undefined;
let sum2;
let add;
function addAgian(a, b) {
  return a + b;
}
let num2;
let sum;

//Execution phase
num1 = 21;
sum2 = addAgain(num1, num2, 4, 5, 6);
add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
num2 = 200;
sum = add(num1, num2, 4, 5, 6);

11. function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
  return a + b;
};

// Your code goes here
//Declaration phase
function test(a) {
  let num1 = 21;
  return add(a, num1);
}
let sum;
let add;

//Execution phase
sum = test(100);
add = (a, b) => {
  return a + b;
};

12. function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

function add(a, b) {
  return a + b;
}

// Your code goes here
//Declaration phase
function test(a) {
  let num1 = 21;
  return add(a, num1);
}
let sum;
function add(a, b) {
  return a + b;
}

//Execution phase
sum = test(100);