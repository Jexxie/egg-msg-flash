# eggjs-msg-flash

[![NPM version][npm-image]][npm-url]
[![build status][travis-image]][travis-url]
[![Test coverage][codecov-image]][codecov-url]
[![David deps][david-image]][david-url]
[![Known Vulnerabilities][snyk-image]][snyk-url]
[![npm download][download-image]][download-url]

[npm-image]: https://img.shields.io/npm/v/eggjs-msg-flash.svg?style=flat-square
[npm-url]: https://npmjs.org/package/eggjs-msg-flash
[travis-image]: https://img.shields.io/travis/eggjs/eggjs-msg-flash.svg?style=flat-square
[travis-url]: https://travis-ci.org/eggjs/eggjs-msg-flash
[codecov-image]: https://img.shields.io/codecov/c/github/eggjs/eggjs-msg-flash.svg?style=flat-square
[codecov-url]: https://codecov.io/github/eggjs/eggjs-msg-flash?branch=master
[david-image]: https://img.shields.io/david/eggjs/eggjs-msg-flash.svg?style=flat-square
[david-url]: https://david-dm.org/eggjs/eggjs-msg-flash
[snyk-image]: https://snyk.io/test/npm/eggjs-msg-flash/badge.svg?style=flat-square
[snyk-url]: https://snyk.io/test/npm/eggjs-msg-flash
[download-image]: https://img.shields.io/npm/dm/eggjs-msg-flash.svg?style=flat-square
[download-url]: https://npmjs.org/package/eggjs-msg-flash

<!--
Description here.
-->

## Install

```bash
$ npm i eggjs-msg-flash --save
```

## Usage

```js
// {app_root}/config/plugin.js
exports.msgFlash = {
  enable: true,
  package: 'eggjs-msg-flash',
};
```

## Configuration

```js
// {app_root}/config/config.default.js
exports.msgFlash = {
};
```

see [config/config.default.js](config/config.default.js) for more detail.

## Example

<!-- example here -->

```
ctx.flash = {
    type: 'success',
    message: {
        some: 'one'
    }
}

// or

ctx.flash_success({some:'one'})

ctx.flash_error()
ctx.flash_info()
ctx.flash_warning()

ctx.request.flash(type, message)

// get message by

ctx.flash
```

## Questions & Suggestions

Please open an issue [here](https://github.com/eggjs/egg/issues).

## License

[MIT](LICENSE)
