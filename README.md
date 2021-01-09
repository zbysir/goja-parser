# goja-parser
Package goja-parse is a JavaScript parser written natively in Go.

This project was largely inspired by [goja](https://github.com/dop251/goja)

Unlike Goja, this package only has the parse function, because I added some es6 features for parser, but it is too complicated for me to interpret it;

### Added syntax
- [Spread_syntax](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)
  - For function calls:
    ```
    myFunction(...iterableObj); // pass all elements of iterableObj as arguments to function myFunction
    ```
  - For array literals or strings:
    ```
    [...iterableObj, '4', 'five', 6]; // combine two arrays by inserting all elements from iterableObj
    ```
  - For object literals (new in ECMAScript 2018):
    ```
    let objClone = { ...obj }; // pass all key:value pairs from an object 
    ```
