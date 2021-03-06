# node-randomuser

[![Build Status](https://img.shields.io/travis/KevinTCoughlin/node-randomuser.svg?style=flat-square)](https://travis-ci.org/KevinTCoughlin/node-randomuser)
[![npm version](https://img.shields.io/npm/v/randomuser.svg?style=flat-square)](https://www.npmjs.com/package/randomuser)

## Installation

Install using the node.js package manager [npm](http://npmjs.org/):

    $ npm install randomuser

## Examples

Demos of the randomuser module are located in: [./examples](https://github.com/KevinTCoughlin/node-randomuser/tree/master/examples)

## Usage

### Require Module and Initialize Client

```javascript
var RandomUser = require('..')
  , r = new RandomUser();
```

### .getUsers(callback)

```javascript
r.getUsers(function(data) {
  console.log(data);
});
```

### .getUsers(params, callback)

```javascript
r.getUsers({ seed: "foxie", results: 5, gender: "male" }, function(data) {
  console.log(data);
});
```

### params {Object} [Documentation](http://randomuser.me/)

* `results` - int specifying number of results to return
* `genders` - string - "male" or "female" specifying gender to generate
* `seed` - string - service will return same data for given seed

## Testing

Issue the following Make command in the top directory to run the mocha.js test cases:

    $ make test

Or...

    $ npm test

## Contributing

Feel free to contribute!

## License

node-randomuser: Copyright (c) 2013-2016 Kevin Coughlin <kevintcoughlin@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
