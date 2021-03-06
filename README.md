> JavaScript's missing ___parseBool___

![](https://img.shields.io/badge/parseBool-JS-267bee.svg?style=flat-square)
[![NPM Downloads](http://img.shields.io/npm/dm/parsebool.svg?style=flat-square)](https://www.npmjs.org/package/parsebool)
[![Build Status][TravisLogo]][Travis]

# Install
```
npm install parsebool
```

# Usage

```js
var parseBool = require("parsebool")
```

```js
parseBool("true")   // => true
parseBool("false")  // => false
parseBool("maybe")  // => "maybe"

// Ignore Case
parseBool("TRUE", { ignoreCase: true })   // => true
parseBool("False", { ignoreCase: true })  // => false

// Negate the value!
parseBool.not("false")  // => true
parseBool.not("true")   // => false
parseBool.not("maybe")  // => "maybe"

```

# License

[MIT][MIT] © [Jorge Bucaran][Author]



[Author]: http://about.bucaran.me

[MIT]: http://opensource.org/licenses/MIT

[TravisLogo]: http://img.shields.io/travis/bucaran/parsebool.svg?style=flat-square

[Travis]: https://travis-ci.org/bucaran/parsebool
