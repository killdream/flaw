Flaw
====

[![Build Status](https://secure.travis-ci.org/robotlolita/flaw.png?branch=master)](https://travis-ci.org/robotlolita/flaw)
[![NPM version](https://badge.fury.io/js/flaw.png)](http://badge.fury.io/js/flaw)
[![Dependencies Status](https://david-dm.org/robotlolita/flaw.png)](https://david-dm.org/robotlolita/flaw)
[![stable](http://hughsk.github.io/stability-badges/dist/stable.svg)](http://github.com/hughsk/stability-badges)

Lightweight and simple error creation in JavaScript.

[![browser support](http://ci.testling.com/robotlolita/flaw.png)](http://ci.testling.com/robotlolita/flaw)


### Example

```js
var flaw = require('flaw')

// Simple error creation
var ParsingError = flaw('ParsingError')
throw ParsingError('Unknow token at...', { line: 1 })

// Raising errors in an expression
n > 0 ? m / n
      : raise(flaw('DivideByZero', 'Can\'t divide by 0'))
```


### Installation

```bash
$ npm install flaw
```


### Documentation

```bash
$ npm install -g calliope
$ calliope build
```

Then open `docs/api/index.html` in your browser.


### Licence

MIT/X11. ie.: do whatever you want.
