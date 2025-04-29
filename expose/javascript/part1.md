# Lab 4: Expose JS Part 1

1. Line 9 prints 'values added: 20'.
2. Line 13 prints 'final result: 20'.
3. We should *never* use var, as seen in this code snippet, because even though we defined the `result` variable WITHIN the if block, we can read, modify, etc. this `result` variable from anywhere within the function scope, as seen when we can execute line 13, calling `console.log('final result: ', result);`. This can lead to confusion where we may erroneously access or modify variables that we thought were out of scope, which may cause errors when we incorrectly track which variables are read and modified in what contexts.
4. Line 9 prints 'values added: 20'.
5. Line 13 causes a `ReferenceError: result is not defined`. This is as we use the `let` keyword to define the `result` variable. Therefore, we can only access `result` within its block scope, which would be only code within the `if` block. Therefore, when we have left the `if` block by line 13, and we try to access `result` by calling `console.log('final result: ', result);`, `result` is no longer accessible in our scope, causing an error.
6. Line 9 causes a `TypeError: Assignment to constant variable`. This is as we declared `result` with the `const` keyword, meaning that we cannot change the value of `result` after initialization. However, in line 9 we attempt to modify the value of `result` with `result = num1 + num2;`, causing our error.
7. Line 13 will not execute as line 9 already causes an error and will terminate the program execution. However, if the error in line 9 were fixed, line 13 would cause a `ReferenceError`, as the `const` keyword is block scoped, so by the time we have reached line 13, we have left the `if` block where `result` was defined, meaning `result` is inaccessible, casuing an error.
