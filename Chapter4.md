The Sum of a Range
```
function range(start, end){
var array = [];
for(var i = start; i <= end; i++){
array.push(i);
}
return array;
}
function sum(array){
var sum = 0;
for(var i = 0; i < array.length; i++){
sum += array[i];
}
return sum; 
}
console.log(sum(range(1, 10)));
```
