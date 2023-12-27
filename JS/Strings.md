
## Copy text to clipboard
``` js
navigator.clipboard.writeText(text);
```

## Capitalize Text
```js
const capitalize = (str) => `${str.charAt(0).toUpperCase()}${str.slice(1)}`;
```

## Get the mouse selection
``` js
const getSelectedText = () => window.getSelection().toString()
getSelectedText()
```