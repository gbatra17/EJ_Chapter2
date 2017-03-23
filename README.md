# EJ_Chapter2

Looping a Triangle: 
```
var hash = '#';
for(var count = 0; count < 7; count++){ 
    console.log(hash);
    hash += "#";
}
```

FizzBuzz:
```
for(var count = 1; count <= 100; count++){ 
  if(count%5 === 0 && count%3 === 0){
    console.log("FizzBuzz");
  } else if(count%3 === 0){
    console.log("Fizz");
  } else if(count%5 === 0 && !count%3 === 0){
    console.log("Buzz");
  }  else {console.log(count);}
}
```

Chess-Board:
```
function chessboard(size){
  var string = "";
  for (var y = 1; y <= size; y++) {   
  for (var x = 1; x <= size; x++) {
    if ((x + y) % 2 === 0)
      string += " ";
    else
      string += "#";
  }
  string += "\n";
  }
console.log(string);  
}
chessboard(8);
```
