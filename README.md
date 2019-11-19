# Javascript Tricks

### Flatten an array of arrays with ```.flat(depth)``` 


```js 
[1,2,3,4,5,[6,7,8]].flat()
//[1,2,3,4,5,6,7,8]

[1,2,3,[4,5,6,[7,8,9]]].flat(2)
//[1,2,3,4,5,6,[7,8,9]]

[1,2,3,[4,5,6,[5,3,6,[3,2,63]]]].flat(Infinity)
//[1,2,3,4,5,6,5,3,6,3,2,63]
```

### Copy arrays and objects with spread operator
```js
let arr = [1,2,3,4,5]
let arr2 = [...arr]

let obj = {
  x: 10,
  y: 20
}
let obj2 = {...obj}
```

### Remove duplicates in an array
```js
let arr = [1,2,2,3,4,4,5]
let noDuplicates = [...new Set(arr)]
```



### Get index and value while looping over an array ES6 Style
```js
let arr = [1,2,3,4,5]
for (const [index, value] of arr.entries()){
  console.log(index, value)
}
```

### Destructuring function arguments
```js
const printName = ({ name }) => {
  console.log(name);
};

const obj = {
  name: 'tyler',
  age: 24
};

printName(obj);
```

### Convert String to DOM Nodes
```js
let getNodes = str => new DOMParser().parseFromString(str, 'text/html').body.childNodes;
```
