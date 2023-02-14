Understanding Scope and the difference between var, let and const
Watch this video before doing the exercise: https://www.youtube.com/watch?v=XgSjoHgy3Rk

1. Guess the output:
let firstName = 'Arya';
const lastName = 'Stark';
var knownAs = 'no one';

console.log(
  window.firstName,
  window.lastName,
  window.knownAs
);

//undefined,undefined,'no one'


2. Guess the output:

let firstName = 'Arya';
const lastName = 'Stark';
var knownAs = 'no one';

function fullName(a, b) {
  return a + b;
}

console.log(window.fullName(firstName, lastName));// AryaStark



3. Make a Execution Context Diagram for the following JS and write the output.

function addOne(num){
  return num + 1;
}
var one = addOne(0);
var two = addOne(1);
console.log(one, two);//1,2


4. Make a Execution Context Diagram for the following JS and write the output.

var one = addOne(0);
function addOne(num){
  return num + 1;
}
var two = addOne(1);
console.log(one, two);//1,2



5. Make a Execution Context Diagram for the following JS and write the output.

console.log(addOne(0));//1
function addOne(num){
  return num + 1;
}
var two = addOne(1);
console.log(two);//2


6. Make a Execution Context Diagram for the following JS and write the output.

var one = addOne(0);// addOne not defined 
const addOne = (num) => {
  return num + 1;
};
var two = addOne(1);
console.log(two);//2


3. Make a Execution Context Diagram for the following JS and write the output.

console.log(addOne(0));// addOne not defined
const addOne = (num) => {
  return num + 1;
};
var two = addOne(1);
console.log(two);//2



4. What will be the output of the following

function isAwesome() {
  var awesome;
  if (false) {
    awesome = true;
  }
  console.log(awesome);
}
isAwesome();//undefined


5. What will be the output of the following

function isAwesome() {
  let awesome;
  if (true) {
    awesome = true;
  }
  console.log(awesome);
}
isAwesome();//true


6. What will be the output of the following
function isAwesome() {
  var awesome;
  if (false) {
    awesome = true;
  }
  console.log(awesome);
}
isAwesome();//undefined



7.  What will be the output of the following

let firstName = 'Arya';
const lastName = 'Stark';
var knownAs = 'no one';

function fullName(a, b) {
  return a + b;
}
const name = fullName(firstName, lastName);
console.log(name);//AryaStark


8. Guess the output of the code below with a reason.
function sayHello() {
  let name = 'Arya Stark';
}
sayHello();//undefined

console.log(name);//name is not define



9. Guess the output of the code below with a reason.
if (true) {
  var name = 'Arya Stark';
}
console.log(name);//Arya Stark


10. Guess the output of the code below with a reason.
if (true) {
  let name = 'Arya Stark';
}
console.log(name);//name is not defined



11.  Guess the output of the code below with a reason.
for (var i = 0; i < 20; i++) {
  //
}
console.log(i);//20


12. Guess the output of the code below with a reason.
for (let i = 0; i < 20; i++) {
  //
}
console.log(i);//i is not defined




13.  Guess the output and the reason behind that.

function sample() {
  if (true) {
    var username = 'John Snow';
  }
  console.log(username);
}
sample();//John Snow



14.   Guess the output and the reason behind that.
function sample() {
  if (true) {
    let username = 'John Snow';
  }
  console.log(username);
}
sample();//username is not defined



15. Guess the output and the reason behind that.

function sample() {
  var username = 'Arya Stark';
  if (true) {
    var username = 'John Snow';
    console.log(username);
  }
  console.log(username, 'second');
}
sample();// output
//John Snow 
//John Snow second


16. Guess the output and the reason behind that.
function sample() {
  let username = 'Arya Stark';
  if (true) {
    let username = 'John Snow';
    console.log(username, 'first');
  }
  console.log(username, 'second');
}
sample();//Output
//John Snow first
//Arya Stark second


17. Guess the output and the reason behind that.
function sample(...args) {
  for (let i = 0; i < args.length; i++) {
    let message = `Hello I am ${args[i]}`;
    console.log(message);
  }
}

sample('First', 'Second', 'Third');//Output
//Hello I am First
//Hello I am Second
//Hello I am Third



18. Guess the output and the reason behind that.
function sample(...args) {
  for (let i = 0; i < args.length; i++) {
    const message = `Hello I am ${args[i]}`;
    console.log(message);
  }
}

sample('First', 'Second', 'Third');//Output
//Hello I am First
//Hello I am Second
//Hello I am Third



19.  Guess the output and the reason behind that.
if (true) {
  const myFunc = function () {
    console.log(username, 'Second');
  };
  console.log(username, 'First');
  let username = 'Hello World!';
  myFunc();// cannot access before initialization
}


20. Guess the output and the reason behind that.

function outer() {
  let movie = 'Mad Max: Fury Road';
  function inner() {
    console.log(
      `I love this movie called ${movie.toUpperCase()}`
    );
  }
  inner();
}

outer();//Output
//I love this movie called MAD MAX: FURY ROAD


21. Guess the output and the reason behind that.

function outer() {
  let movie = 'Mad Max: Fury Road';
  function inner() {
    let movie = 'Before Sunrise';
    console.log(
      `I love this movie called ${movie.toUpperCase()}`
    );
  }
  inner();
}

outer();//Output
//I love this movie called BEFORE SUNRISE

22. Guess the output and the reason behind that.

function outer() {
  let movie = 'Mad Max: Fury Road';
  function inner() {
    let movie = 'Before Sunrise';
    function extraInner() {
      let movie = 'Gone Girl';
      console.log(
        `I love this movie called ${movie.toUpperCase()}`
      );
    }
    extraInner();
  }
  inner();
}
outer();//Output
//I love this movie called GONE GIRL


23. Using reduce find the final value when the initial value passed is 100. You have to pass the output of one function into the input of next function in the array allFunctions starts with addOne ends with half.

const addOne = (num) => {
  return num + 1;
};
const subTwo = (num) => {
  return num - 2;
};
const multiplyThree = (num) => {
  return num * 3;
};
const half = (num) => {
  return num / 2;
};

let allFunctions = [
  addOne,
  subTwo,
  multiplyThree,
  addOne,
  multiplyThree,
  half,
];


allFunctions.reduce((acc,cv)=>{
   acc=cv(acc);
  console.log(acc)
  return acc;
},100);
//Output 
447