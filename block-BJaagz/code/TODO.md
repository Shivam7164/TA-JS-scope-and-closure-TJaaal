Implement forEach array method using Array.reduce
forEach accepts two parameter array and callback
It does not return anything
It should work exactly like array forEach method

// Your code goes here
function map(arr , cb){
   return arr.reduce((acc , cv,i,arr) =>{
       cb(cv,i,arr)
    }) 
 }
map(["sam","shiavm","jhon"] , (n,i,arr)=> console.log(n+n)) 
output //shiavmshiavm
//jhonjhon 



Implement map array method using Array.reduce
map accepts two parameter array and callback
It returns same size of array
It should work exactly like array map method

  // Your code goes here
function map(arr , cb){
   return arr.reduce((acc , cv,i,arr) =>{
       acc.push(cb(cv,i,arr)) 
        return acc;
    },[])
    
 }
map(["sam","shiavm","jhon"] , (n)=> n+n)// ['samsam', 'shiavmshiavm', 'jhonjhon']
Implement filter array method using Array.reduce
filter accepts two parameter array and callback
It returns same size or smaller array
It should work exactly like array filter method
  // Your code goes here
 
function map(arr , cb){
   return arr.reduce((acc , cv,i,arr) =>{
       if(cb(cv,i,arr)){
       acc.push(cv) 
       }
        return acc;
    },[])
    
 }
 map(["sam","shiavm","jhon"] , (n)=> n.startsWith("s"))