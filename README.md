# URL

---

Uniform Resource Locator.

---

## 使用说明

```js
var Url = require("url");

var url = new Url("https://www.example.com/path/to/page?pa=A1&pa=A2&pb=B#hash");
console.log(url);
console.log(url.getParam("pa")); // "A1"
console.log(url.getParams("pa")); // ["A1", "A2"]
```

## API

### new Url(String url)

Constructor.

### String getParam(String name)

Get named `name` param string the first.

### Array getParams(String name)

Get named `name` params string of all.

### Url delParam(String name)

Delete named `name` params.

### Url addParam(String name, String|Array value)

Add params named `name`.

### Url setParam(String name, String|Array)

Add or replace param values named `name`.
