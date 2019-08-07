# Javascript Tricks

### Flatten an array of arrays with ```.flat(depth)``` 


```js [1,2,3,4,5,[6,7,8]].flat()``` &#8594
```[1,2,3,4,5,6,7,8]```

```js[1,2,3,[4,5,6,[7,8,9]]].flat(2)```
```=> [1, 2, 3, 4, 5, 6, [7,8,9]]```
