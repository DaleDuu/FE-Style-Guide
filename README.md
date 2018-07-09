# JavaScript Style Guide

## Table of Contents
1. [Types](#types)
1. [Format](#format)

## Types
If you reassign ferences, use `let` instead of `var`. eslint: [`no-var`](https://eslint.org/docs/rules/no-var.html)

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
