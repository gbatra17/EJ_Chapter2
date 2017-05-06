<h1> Chapter 3 </h1>

Minimum
```
function min(num1, num2){
  if(num1>=num2){
    return num2;
  } else {
    return num1;
  }
}
console.log(min(0,10));
console.log(min(0, -10));
```
Recursion
```
function isEven(num){
 num = Math.abs(num);
if(num === 0){
return true;
} else if(num === 1){
  return false;
} else {
  return isEven(num - 2);
}
}
```

Bean Counting
//In this task we are asked to create a function that inputs a string and outputs the number of times a character appears in the string. 
```
function countBs(string){
var splitString = string.split('');
var count = 0;
splitString.forEach(function(char){
  if(char === 'B'){
    count++;
}});
return count;
}

function countChar(string, char){
var splitString = string.split('');
var count = 0;
splitString.forEach(function(e){
  if(e === char){
    count++;
}});
return count;
}

//Using countChar as an innerfunction to re-define countBs.
function rewrittenCountBs(string){
return countChar(string, 'B');
}

console.log(countBs("BBC"));
// → 2
console.log(countChar("kakkerlak", "k"));
// → 4
console.log(rewrittenCountBs("BBC"));
// 2
```
