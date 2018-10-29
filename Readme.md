
# koa-format-logger

控制台输出格式如下：

```
  <-- req  GET /dist/web.app.js 2018-10-29 20:51:05
  --> res  GET /dist/web.app.js 200 3ms 10.26mb
  <-- req  GET /dist/web.27.js 2018-10-29 20:51:05
  --> res  GET /dist/web.27.js 200 1ms 29.82kb
  <-- req  GET /dist/web.57.js 2018-10-29 20:51:05
  --> res  GET /dist/web.57.js 200 2ms 36.16kb

```

## Installation

```js
$ npm install koa-format-logger
```

## Example

```js
const logger = require('koa-format-logger')
const Koa = require('koa')

const app = new Koa()
app.use(logger())
```


