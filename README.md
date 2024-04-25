# @wemnyelezxnpm/odio-dignissimos-corporis <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Get the ArrayBuffer out of a TypedArray, robustly.

This will work in node <= 0.10 and < 0.11.4, where there's no prototype accessor, only a nonconfigurable own property.
It will also work in modern engines where `TypedArray.prototype.buffer` has been deleted after this module has loaded.

## Example

```js
const typedArrayBuffer = require('@wemnyelezxnpm/odio-dignissimos-corporis');
const assert = require('assert');

const arr = new Uint8Array(0);
assert.equal(arr.buffer, typedArrayBuffer(arr));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@wemnyelezxnpm/odio-dignissimos-corporis
[npm-version-svg]: https://versionbadg.es/inspect-js/@wemnyelezxnpm/odio-dignissimos-corporis.svg
[deps-svg]: https://david-dm.org/inspect-js/@wemnyelezxnpm/odio-dignissimos-corporis.svg
[deps-url]: https://david-dm.org/inspect-js/@wemnyelezxnpm/odio-dignissimos-corporis
[dev-deps-svg]: https://david-dm.org/inspect-js/@wemnyelezxnpm/odio-dignissimos-corporis/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@wemnyelezxnpm/odio-dignissimos-corporis#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@wemnyelezxnpm/odio-dignissimos-corporis.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@wemnyelezxnpm/odio-dignissimos-corporis.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@wemnyelezxnpm/odio-dignissimos-corporis.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@wemnyelezxnpm/odio-dignissimos-corporis
[codecov-image]: https://codecov.io/gh/inspect-js/@wemnyelezxnpm/odio-dignissimos-corporis/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@wemnyelezxnpm/odio-dignissimos-corporis/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@wemnyelezxnpm/odio-dignissimos-corporis
[actions-url]: https://github.com/inspect-js/@wemnyelezxnpm/odio-dignissimos-corporis/actions
