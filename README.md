Flaw
====

Lightweight and simple error creation in JavaScript.


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
