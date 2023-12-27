
## Remove duplicates from array
``` js
const uniqueArray = [...new Set(array)];
```

## Random btwn two values
``` js
const randomNumber = Math.floor(Math.random() * (max - min + 1)) + min;
```

## How to Sort Elements By Certain Property
```js
const sortBy = (arr, key) => arr.sort((a, b) => a[key] > b[key] ? 1 : a[key] < b[key] ? -1 : 0);
```
