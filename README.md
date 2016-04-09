lightscript
===========

Functional JavaScript-compatible programming language

  * Subset of ES3
  * Import external JavaScript 
  * Type annotations

Type annotations
----------------

To keep ES3 compatibility, type annotations can be expressed as comments

```js
//@: a -> a
var identity = function (value) {
  return value;
};
```


Type annotations will be applied to the next function expression found

Inline annotations are also valid

```js
var api = {
  identity: /*@: a -> a */ function (value) {
    return value;
  }
};
```

### References

  * [Ramda](http://ramdajs.com/)
  * [TypeScript](https://www.typescriptlang.org/)
  * [JSON Schema](http://json-schema.org/)
  * [Elm](http://elm-lang.org/)
  * [Haskell](https://www.haskell.org/)

Spec
----

### Built-in objects

<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects>

  * `module`

### Expressions and operators

<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators>

Primary expressions

  * `function`: function expression
  * `[]`: array initializer
  * `{}`: object initializer
  * `()`: grouping operator

Left-hand-side expressions

  * `object['property']`: property accessors

Unary operators

  * `!`: logical not

Arithmetic operators

  * `+`: addition
  * `-`: substraction
  * `*`: multiplication
  * `/`: division
  * `%`: remainder

Relational operators

  * `<`: less than
  * `>`: greater than
  * `<=`: less than or equal
  * `>=`: greater than or equal

Equality operators

  * `===`: identity
  * `!==`: non-identity

Binary logical operators

  * `&&`: and
  * `||`: or

Assignment operators

  * `=`: assignment

### Statements and declarations

<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements>

Control flow

  * `{}`: block
  * `if...else`: executes a statement if expression is true
  * `throw`: throws a user-defined exception
  * `try...catch`: mark a block of statements to try

Declarations

  * `var`: declares a variable, optionally initializing it to a value

Functions and classes

  * `return`: specifies the value to be returned
