# Javascript Tricks

### Flatten an array of arrays with ```.flat(depth)``` 


```js 
[1,2,3,4,5,[6,7,8]].flat()
``` 
→
```[1,2,3,4,5,6,7,8]```

```[1,2,3,[4,5,6,[7,8,9]]].flat(2)``` →
```[1,2,3,4,5,6,[7,8,9]]```

```[1,2,3,[4,5,6,[5,3,6,[3,2,63]]]].flat(Infinity)``` →
```[1,2,3,4,5,6,5,3,6,3,2,63]```

### Remove duplicates in an array
```js
let arr = [1,2,2,3,4,4,5]
let noDuplicates = [...new Set(arr)]
```
