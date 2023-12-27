
## Remove duplicates from array
``` js
const uniqueArray = [...new Set(array)];
```

## Random btwn two values
``` js
const randomNumber = Math.floor(Math.random() * (max - min + 1)) + min;
```

## Copy text to clipboard
``` js
navigator.clipboard.writeText(text);
```

## Capitalize Text
```js
const capitalize = (str) => `${str.charAt(0).toUpperCase()}${str.slice(1)}`;
```

## How to Sort Elements By Certain Property
```js
const sortBy = (arr, key) => arr.sort((a, b) => a[key] > b[key] ? 1 : a[key] < b[key] ? -1 : 0);
```

## Get the mouse selection
``` js
const getSelectedText = () => window.getSelection().toString()
getSelectedText()
```