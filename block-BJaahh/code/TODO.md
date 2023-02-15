Getting to understand closure properly

1. Write a function called multiplyBy that takes a number as an argument and returns a function. Returned function takes another number as an argument and returns the multiplication of both the numbers.
// Your code goes here
function multiplyBy(number){
  return (num)=>{
    return number*num
  }
}

const double = multiplyBy(2);
const final = double(15); // final should be 30


2. Write a function called fullName that takes a string firstName as an argument and returns a function. Returned function takes another string lastName as an argument and returns full name.
// Your code goes here

function fullName(fn){
  return (ln)=> `${fn} ${ln}`
}

const name = fullName('Will');
const final = name('Smith'); // final should be "Will Smith"


3. Write a function called isInBetween which takes two parameter a and b and returns a function. When you call the returned function with any number it returns true if the value is in between a and b.
function isInBetween(a, b) {
  return function between(num){
    // if(a<=num && num<=b){
    //   return true;
    // }else{
    //     return false;
    // }
      return a<=num && num<=b
  }
}

const isChild = isInBetween(10, 100);
isChild(21); // true
isChild(45); // true
isChild(103); // false


4. Write a function call letsWishThem that take one parameter string called greeting and returns a function that takes another argument called message.

function letsWishThem(greeting){
  return (called)=>`${greeting} ${called}`
} 


const callWithHey = letsWishThem('Hey');
const callWithHello = letsWishThem('Hello');
callWithHey('Arya'); // Hey Arya
callWithHello('How Are You?'); // Hello How Are You?


5. Write a function called addGame which takes a string (name of the game) and the current score. It returns a function calling that will increment the score by one and print something like Score of Basketball is 1.

function addGame(gameName,curScore) {
  return ()=>`Your score of ${gameName} is ${++curScore}`
}

// Output

const hockey = addGame('Hockey', 0);
hockey(); // Your score of Hockey is 1
hockey(); // Your score of Hockey is 2
const cricket = addGame('Cricket', 1);
cricket(); // Your score of Cricket is 2
cricket(); // Your score of Cricket is 2


6. Write a function called getCard which takes one of these options (club, spade, heart, diamond) returns a function calling that function returns random card (2,3,4,5,6,7,8,9,10,J, Q, K, A) of that suit.

function getCard(suit){
  let randomCard = [2,3,4,5,6,7,8,9,10,"J","Q","K","A"]
  return ()=>{
    let index = Math.floor(Math.random() * randomCard.length)
    return `Card is: ${randomCard[index]} ${suit}`
  } 
}

// Output

const randomClub = getCard('Club');
randomClub(); // Card is: 6 Club
randomClub(); // Card is: A Club
const randomSpade = getCard('Spade');
randomSpade(); // Card is: 6 Spade
randomSpade(); // Card is: A Spade