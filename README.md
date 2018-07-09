# JavaScript Style Guide

## Table of Contents
1. [Types](#types)
1. [Format](#format)

## Types
 <a name="types--references"></a><a name="1.1"></a>
 - [1.1](#types--references) If you reassign references, use `let` instead of `var`. eslint: [`no-var`](https://eslint.org/docs/rules/no-var.html)

    > `let` is block-scoped rether than function-scoped like `var`.

    ```javascript
    // bad
    var maxPage = 1;
    var answerType = 1;
    if (answerType) {
      maxPage += 1;
    }

    // good
    let maxPage = 1;
    const answerType = 1;
    if (answerType) {
      maxPage += 1;
    }
    ```
    
 <a name="types--propTypes"></a><a name="1.2"></a>
 - [1.2](#types--propTypes) Avoid use object in array for propTypes

    > `let` is block-scoped rether than function-scoped like `var`.

    ```javascript
    // bad
    var maxPage = 1;
    var answerType = 1;
    if (answerType) {
      maxPage += 1;
    }

    // good
    let maxPage = 1;
    const answerType = 1;
    if (answerType) {
      maxPage += 1;
    }
    ```
    
## Format    
  <a name="format-object-shorthand"></a><a name="2.1"></a>
  - [2.1](#format-object-shorthand) Use property value shorthand. eslint: [`object-shorthand`](https://eslint.org/docs/rules/object-shorthand.html)

    > It is shorter to write and descriptive.

    ```javascript
    const benchmark = 'benchmark';

    // bad
    const obj = {
      benchmark: benchmark,
    };

    // good
    const obj = {
      benchmark,
    };
    ```
