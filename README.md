=========
Proxy.js
=========

![](https://travis-ci.org/uupaa/Proxy.js.png)

XMLHttpRequest proxy.

# Document

- [WebModule](https://github.com/uupaa/WebModule) ([Slide](http://uupaa.github.io/Slide/slide/WebModule/index.html))
- [Development](https://github.com/uupaa/WebModule/wiki/Development)
- [Proxy.js wiki](https://github.com/uupaa/Proxy.js/wiki/Proxy)


# How to use

```js
<script src="lib/Proxy.js">
<script>
// for Browser
var proxy = new Proxy();

proxy.get("./index.html", function(error, responseText, xhr) {
    console.log(responseText);
});

</script>
```

```js
// for WebWorkers
importScripts("lib/Proxy.js");

var proxy = new Proxy();

proxy.get("./index.html", function(error, responseText, xhr) {
    console.log(responseText);
});
```
