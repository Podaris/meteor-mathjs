![math.js](https://raw.github.com/josdejong/mathjs/master/img/mathjs.png)

[http://mathjs.org](http://mathjs.org) Original Documentation

Math.js is an extensive math library for JavaScript and Node.js.
It features a flexible expression parser and offers an integrated solution
to work with numbers, big numbers, complex numbers, units, and matrices.
Powerful and easy to use.


## Features

- Supports numbers, big numbers, complex numbers, units, strings, arrays, and matrices.
- Is compatible with JavaScript's built-in Math library.
- Contains a flexible expression parser.
- Supports chained operations.
- Comes with a large set of built-in functions and constants.
- Has no dependencies. Runs on any JavaScript engine.
- Can be used as a command line application as well.
- Is easily extensible.


## Usage

Math.js can be installed using Meteor add.

    meteor add ecwyne:mathjs

Math.js can be used similar to JavaScript's built-in Math library. Besides that,
math.js can evaluate
[expressions](http://mathjs.org/docs/expressions.html)
and supports
[chained operations](http://mathjs.org/docs/chained_operations.html).

```js

// functions and constants
math.round(math.e, 3);            // 2.718
math.atan2(3, -3) / math.pi;      // 0.75
math.log(1000, 10);               // 3
math.sqrt(-4);                    // 2i
math.pow([[-1, 2], [3, 1]], 2);   // [[7, 0], [0, 7]]

// expressions
math.eval('12 / (2.3 + 0.7)');    // 4
math.eval('5.08 cm to inch');     // 2 inch
math.eval('sin(45 deg) ^ 2');     // 0.5
math.eval('9 / 3 + 2i');          // 3 + 2i
math.eval('det([-1, 2; 3, 1])');  // -7

// chained operations
math.select(3)
    .add(4)
    .multiply(2)
    .done(); // 14
```


## Documentation

- [Examples](http://mathjs.org/examples/index.html)
- [Overview](http://mathjs.org/docs/index.html)
- [History](http://mathjs.org/history.html)


## License

Copyright (C) 2013-2014 Jos de Jong <wjosdejong@gmail.com>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
