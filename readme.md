### isInPage ([from MDN](https://developer.mozilla.org/en-US/docs/Web/API/Node/contains))


#### Example

This function checks to see if an element is in the page's body. As contains is inclusive and determining if the body contains itself isn't the intention of isInPage this case explicitly returns false.

```js
function isInPage (node) {
  return (node === document.body) ? false : document.body.contains(node)
}
```

#### npm usage

```js
var isInPage = require('is-in-page')
if (isInPage(document.getElementById('wow'))) {
  console.log('cool')
}

```
[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)
