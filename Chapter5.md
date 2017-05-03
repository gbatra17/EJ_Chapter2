Flattening
```
var arrays = [[1,2,3], [4,5], [6]];
arrays.reduce(function(array){
return array.concat(array);
});
```
