# Type Coercion in JavaScript Addition
This example demonstrates the unexpected behavior of JavaScript's addition operator (+) when dealing with different data types.  JavaScript performs type coercion implicitly, which can lead to unexpected results if not handled carefully. This is especially true when adding numbers with strings or booleans.

## Bug
The `foo` function is designed to add two numbers. However, due to type coercion, the function produces unexpected results when passed strings or booleans. The addition operation concatenates the strings instead of performing numerical addition.  With booleans, true is coerced to 1 and false to 0.

## Solution
The solution involves using explicit type conversion to ensure numerical addition.  The `Number()` function can be used to convert the arguments to numbers before performing the addition operation. This ensures consistent behavior, regardless of input data types.