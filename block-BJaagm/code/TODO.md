What does thread of execution means in JavaScript? when javascript engine execute the code line by line is called thread of execution

Where the JavaScript code gets executed? Javascript code gets executed inside global execution context

What does context means in Global Execution Context? context means environment in which you are execute the code

When do you create a global execution context. whenever the javascript engine run your code then create first exicution context

Execution context consists of what all things?

What are the different types of execution context? global and function execution context

When global and function execution context gets created? globle execution context is the first exicution context that created by javascript engine whenever running your code for the first time but

function execution create whenever we execute the function

Function execution gets created during function execution or while declaring a function. when call the function that time create function execution

Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named img. Use ![](./img/image-name.png) to display it here.



var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
<!-- ![](./imgs/ans1) -->



var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
<!-- ![](./img/ans2) -->



var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
<!-- ![](./imgs/ans3.jpg) -->