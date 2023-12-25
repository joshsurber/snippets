#js
``` js
const fetchAPI = async(URL) => {
	const response = await fetch(URL);
	
	const data = await response.json();
	
	console.log(data)
}
fetchAPI("https://foo.bar/baz.quux")
```