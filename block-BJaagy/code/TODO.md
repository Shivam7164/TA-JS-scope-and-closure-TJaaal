Create a function by your choice that accepts a callback function.
function higherOrderFn(cb){
    return cb(21)
}
function callBack(v){
    return v+1
}
higherOrderFn(callBack)
Create a function by you choice that returns a function reference.

function higherOrderFn(cb){
    return cb 
}
function callBack(v){
    return v+1
}
higherOrderFn(callBack)

Create a higher order function called map that takes two inputs:
An array of numbers/string/boolean etc
A 'callback' function - a function that is applied to each element of the array (inside of the function 'map')
Have map return a new array filled with values that are the result of the 'callback' function on each element of the input array.
// Your code goes here
let array = [1,2,3,4,5]
function map(arr cb){
    let final = []
  for(let ele of arr){
    final.push(cb(ele))
  }
}
function callBackFn(a){
    return a*2
}
let addFive = map(array , callBackFn)
// Test Your Code
console.log(addFive)


Create a higher-order function called forEach taht takes an array and a callback, and runs the callback on each element of the array. forEach does not return anything.
// Your code goes here

let array = [1,2,3,4,5]
function forEach(arr , cb){
 let arrData = []
 for(let a of arr){
 arrData.push(cb(a))
 }
}
function callBackFn(v){
    return v+5
}
let addFive = forEach(array,callBackFn)
console.log(addFive) // undefined


Create higher-order function called filter takes an array and a callback, and runs the callback on each element of the array if the return value of callback is truthy store in new array return the new array.
// Test Your Code
let array = [21,34,6,88,43,57]
function filler(arr , cb){
    let filterValue = []
  for(let a of arr){
    if(a%2 == 0){
        filterValue.push(cb(a))
    }
  }
  return filterValue
}
function callBackFn(value){
 if(value%2 == 0){
     return value;
 }
}
let trueValue = filler(array , callBackFn)
console.log(truevalue)
