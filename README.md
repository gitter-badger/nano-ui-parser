[![Gitter][gitter-image]][gitter-url]
[![NPM version][npm-image]][npm-url]
[![Build status][travis-image]][travis-url]
[![Test coverage][coveralls-image]][coveralls-url]
[![Dependency Status][david-image]][david-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

# nano-ui-parser
Very simple UI descriptions texts parser

## Usage

```js
	var parse_tree = require('nano-ui-parser');

	var tree = parse_tree(text);

	console.log(tree.toString());
```

## function parse_tree(text)

Returns `Directive` class tree

## class: Directive

* id {String}
* args {String}
* children {Array} of the same class children objects. When object hasn't children its filled with `undefined` value.

## tree.enum(callback)

* function callback(path, args)
  * path {Array} of 'id's
  * args {String} arguments of the node

## About UI files

```
root arguments
  sub-element-1 ererw -> werwer
    sub-sub-element-1 there is any text can be arguments
    sus-sub-element-2
  sub-element-2
    sub-sub-element-1
```

[bithound-image]: https://www.bithound.io/github/Holixus/nano-ui-parser/badges/score.svg
[bithound-url]: https://www.bithound.io/github/Holixus/nano-ui-parser

[gitter-image]: https://badges.gitter.im/Holixus/nano-ui-parser.svg
[gitter-url]: https://gitter.im/Holixus/nano-ui-parser

[npm-image]: https://badge.fury.io/js/nano-ui-parser.svg
[npm-url]: https://badge.fury.io/js/nano-ui-parser

[github-tag]: http://img.shields.io/github/tag/Holixus/nano-ui-parser.svg
[github-url]: https://github.com/Holixus/nano-ui-parser/tags

[travis-image]: https://travis-ci.org/Holixus/nano-ui-parser.svg?branch=master
[travis-url]: https://travis-ci.org/Holixus/nano-ui-parser

[coveralls-image]: https://coveralls.io/repos/github/Holixus/nano-ui-parser/badge.svg?branch=master
[coveralls-url]: https://coveralls.io/github/Holixus/nano-ui-parser?branch=master

[david-image]: https://david-dm.org/Holixus/nano-ui-parser.svg
[david-url]: https://david-dm.org/Holixus/nano-ui-parser

[license-image]: https://img.shields.io/badge/license-MIT-blue.svg
[license-url]: LICENSE

[downloads-image]: http://img.shields.io/npm/dt/nano-ui-parser.svg
[downloads-url]: https://npmjs.org/package/nano-ui-parser
