Which all function is Higher order function and which one is a callback function in the code given below.

let marks = [34, 45, 56, 76];
function multiplyArrayByN(arr, cb) { // higher order function
  let finalArr = [];
  for (let elm of arr) {
    finalArr.push(cb(elm));
  }
  return finalArr;
}
function addFive(n) { // callback function
  return n + 5;
}
function multiplyBy5(n) { // callback function
  return n * 5;
}
let numbersAddedFive = multiplyArrayByN(marks, addFive);
let numbersMultipliedBy5 = multiplyArrayByN(marks, multiplyBy5);

Create the execution context diagram of the above code snippet


Write a higher order function that accepts a number and a operation function (callback function). Call the callback function passing the number as argument and return the returned value.
// your code goes her

function higherOderFn(num , cb){ // higher order function
  return cb(num)
}
function callBackFn(value){ //callback function
    return value + 5
}
let numbersAddedFive = higherOderFn(5,callBackFn)
console.log(numbersAddedFive); // 10


Write a higher order function that accepts a string and a operation function (callback function). Call the callback function passing the string as argument and return the returned value.
  // your code goes her

function higherOrderFn(str,cb){ // 
    return cb(str)
}
function callBackFn(string){
  return (string + ' ' +"rajpoot").toUpperCase()
}

let addStr = higherOrderFn("shivam", callBackFn)
 console.log(addStr) // 'shivam rajpoot'