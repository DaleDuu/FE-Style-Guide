# JavaScript Style Guide

## Table of Contents
1. [Types](#types)

## Types
 <a name="types--references"></a><a name="1.1"></a>
 - [1.1](#references--disallow-var) If you reassign references, use `let` instead of `var`. eslint: [`no-var`](https://eslint.org/docs/rules/no-var.html)

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
