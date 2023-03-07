```javascript
function chunk(array, size = 1) {
  const result = [];
  for (let i = 0; i < array.length; i += size) {
    result.push(array.slice(i, i + size));
  }
  return result;
}
```
Or use this inline-able option where 2 is the chunk size:
```javascript
[1,2,3,4,5].reduce((acc, val) => (2 > acc[acc.length-1].length ? acc[acc.length-1].push(val) : acc.push([val]), acc), [[]]);
```
