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
```
function countChar(string, character){
var array = string.split("");
var count = 0;
for(var i = 0; i < array.length; i++){
  if(array[i] === character){
	count++;
  }
}
return count;
}

countChar("Garima Batra", "a"); // 4

function countBs(string){
return countChar(string, "B");
}
```
