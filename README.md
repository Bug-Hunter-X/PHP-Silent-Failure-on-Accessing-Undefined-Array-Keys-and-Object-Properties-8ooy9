# PHP Silent Failure on Undefined Array Keys and Object Properties

This repository demonstrates a common, yet subtle, bug in PHP: the silent failure when accessing undefined array keys or object properties.  PHP will return `null` without any error or warning, leading to hard-to-find bugs.

## The Problem

PHP's behavior of returning `null` for undefined keys or properties can lead to unexpected results and make debugging more difficult.  This is particularly problematic in large, complex applications.

## The Solution

The solution involves using either the `isset()` function to explicitly check for the existence of a key or property, or using the null coalescing operator (`??`) to provide a default value if the key or property doesn't exist.  This makes your code more robust and less prone to errors.

## How to Run

1. Clone this repository.
2. Run `bug.php` to see the issue.
3. Run `bugSolution.php` to see how to fix the issue.