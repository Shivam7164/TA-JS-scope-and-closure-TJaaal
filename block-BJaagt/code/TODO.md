Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

function hello() {
  var username = 'Arya';
}
console.log(username); // username is not defined

In above code we are looking for the variable named usename. There is no variable named username in the global scope. The variable is inside the function named hello and we can't access the variable defined inside a function from outside.
The above code will throw an error Reference Error username is not defined.


Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.
{
  const username = 'Arya';
}
console.log(useranme); // username is not defined

user name is not defined because username is defined inside the block; so we can not access them 

Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.
if (true) {
  let username = 'Arya';
}
console.log(useranme); // user name is not defined


Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.
if (true) {
  var username = 'Arya';
}
console.log(useranme); // 'Arya'



Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); // username already defined


Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(username); // John


Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(username); // 'John'



Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // 1,2,3,4,5,6,7,8,9
}
console.log(i, 'Second'); 10


Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // 1,2,3,4,5,6,7,8,9
}
console.log(i, 'Second'); i is not defined