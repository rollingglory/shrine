# JavaScript Coding Convention

## Goal

A convention to standardize JavaScript coding style.

## Intro

We are not reinventing the wheels. We adopt from [AirBnB JavaScript Style Guide](https://github.com/airbnb/javascript) and adjust accordingly to our preferences.

In this document, we will rewrite the selected specification we adopt and add a few of our preferences. For anything that is not stated in this document, refer to AirBnB JavaScript Style Guide.

## References

* 2.1 Use `const` for all of your references; avoid using `var`. eslint: [`prefer-const`](https://eslint.org/docs/rules/prefer-const.html), [`no-const-assign`](https://eslint.org/docs/rules/no-const-assign.html)

  > Why? This ensures that you can’t reassign your references, which can lead to bugs and difficult to comprehend code.

  ```javascript
  // bad
  var a = 1;
  var b = 2;

  // good
  const a = 1;
  const b = 2;
  ```

* 2.2 If you must reassign references, use `let` instead of `var`. eslint: [`no-var`](https://eslint.org/docs/rules/no-var.html)

  > Why? `let` is block-scoped rather than function-scoped like `var`.

  ```javascript
  // bad
  var count = 1;
  if (true) {
    count += 1;
  }

  // good, use the let.
  let count = 1;
  if (true) {
    count += 1;
  }
  ```

## Objects

* 3.1 Use the literal syntax for object creation. eslint: [`no-new-object`](https://eslint.org/docs/rules/no-new-object.html)

  ```javascript
  // bad
  const item = new Object();

  // good
  const item = {};
  ```

* 3.3 Use object method shorthand. eslint: [`object-shorthand`](https://eslint.org/docs/rules/object-shorthand.html)

  ```javascript
  // bad
  const atom = {
    value: 1,

    addValue: function (value) {
      return atom.value + value;
    },
  };

  // good
  const atom = {
    value: 1,

    addValue(value) {
      return atom.value + value;
    },
  };
  ```

* 3.4 Use property value shorthand. eslint: [`object-shorthand`](https://eslint.org/docs/rules/object-shorthand.html)

  > Why? It is shorter and descriptive.

  ```javascript
  const lukeSkywalker = 'Luke Skywalker';

  // bad
  const obj = {
    lukeSkywalker: lukeSkywalker,
  };

  // good
  const obj = {
    lukeSkywalker,
  };
  ```

_To be continued. More to come_

