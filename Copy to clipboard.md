#js
```js
document.querySelector('#input-text').select();
document.execCommand('copy');
```

New API (may not be supported in all browsers):

```js
navigator.clipboard.writeText(document.querySelector('#input-text').value);
```