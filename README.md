<h1 align="center">qart.js</h1>
<p align="center">
<a href="https://www.npmjs.com/package/qartjs"><img src="https://img.shields.io/npm/dt/qartjs.svg" alt="Downloads"></a>
<a href="https://www.npmjs.com/package/qartjs"><img src="https://img.shields.io/npm/v/qartjs.svg" alt="Version"></a>
<a href="https://www.npmjs.com/package/qartjs"><img src="https://img.shields.io/npm/l/qartjs.svg" alt="License"></a>
<br>
qart.js merge picture and QR code.
</p>
<img src="intro.png">

## Glance At
https://kciter.github.io/qart.js/

## Installation
```
$ npm install qartjs
```
or clone this repository and copy `qart.min.js` to your project.

## Usage
### In the browser
```html
<script src="../dist/qart.min.js"></script>
<script>
	new QArt({
		value: value,
		imagePath: './example.png',
		filter: filter
	}).make(document.getElementById('qart'));
</script>
```

### In the ES6
```
import QArt from 'qartjs';
const qart = new QArt({
	value: value,
	imagePath: './example.png',
	filter: filter
});
qart.make(document.getElementById('qart'));
```

## Options
|Field|Type|Description|Default|
|-----|----|-----------|-------|
|value|String|The data of the QR code.|*Required*|
|imagePath|String|The path of the combined image.|*Required*|
|filter|String|Define an image filter. `threshold` or `color`|threshold|

## Dependency
* [qrcode](https://github.com/kazuhikoarase/qrcode-generator/tree/master/js)

## Inspire
* [CuteR](https://github.com/chinuno-usami/CuteR)

## TODO
* [ ] Resize feature.
* [ ] Server-Side Rendering.
* [ ] CLI Command.

## LICENSE
[GPLv3](LICENSE)
