# type-check

type-check is a lightweight library to help developers catch bugs before they skitter in by making sure the right types of arguments are being passed into functions and methods.

It couldn't be easier:

```
let typeCheck = require('type-check');

let add = function (a, b) {
  typeCheck(a, 'number');
  typeCheck(b, 'number');

  return a + b;
};

add(3, 4); // 7

add(3, 'four'); // TypeError: Expected argument to be of type "number" but instead received type "string"
```
## Getting Started

#### Step 1
In the terminal:
```
$ npm install type-check
```
#### Step 2
In path/to/my/rad/app/or/whatever/app.js:
```
let typeCheck = require('type-check');
```
#### Step 3
Nope

## Contributing
We'd love contributors and feedback! We are currently at 100% test coverage and that's the way it's gon' be. But for real, hit us up and let's make this thing even better.

## License
type-check is released under the [MIT License](https://opensource.org/licenses/MIT)