# Lab 4: Expose JS Part 2

1. Line 12 prints `i`, which is the amount of iterations that our for loop went through (aka the number of prices that we applied a discount to).
2. Line 13 prints `150`, which is the value of the last price in our list after we've applied a discount to it, prior to rounding to the nearest cent.
3. Line 14 prints `150`, which is the value of the last price in our list after we've applied a discount to it and rounded to the nearest cent.
4. Our function returns our list of prices after we've applied our discount and rounded to the nearest cent in the form of a list. This is as, during function execution, we iterate through each value in our list of prices, apply the discount to it, round to the nearest cent, then add it to our `discounted` list. Then, when we have iterated through every value, we return the `discounted` list.
5. Line 12 causes a `ReferenceError: i is not defined` error, as `i` is defined with the `let` keyword, so it is only available within the `for` block. Calling it in line 12, we have left the scope of the `for` block, now `i` is not defined causing an error.
6. Line 13 causes a `ReferenceError: discountedPrice is not defined` error, as `discountedPrice` is defined with the `let` keyword, so it is only availble within the `for`'s execution block. Calling it on line 13, we have left the scope of `discountedPrice`, so an error is caused.
7. Line 14 prints `150`, which is the value of the last price in our list after we've applied a discount to it and rounded to the nearest cent.
8. This function returns a list of prices after we've applied a and rounded to the nearest cent, in the form of a list. This is as during function execution, we iterate thorugh each value in the list of prices, apply the discount, round to the nearest cent, then add the new price to our `discounted` list. Then, once iterated through every value, we return the `discounted` list.
9. Line 11 causes a `ReferenceError: i is not defined` error, as `i` is defined with the `let` keyword, so it is only available within the `for` block. Calling it in line 11, we have left the scope of the `for` block, now `i` is not defined causing an error.
10. Line 12 prints `3`, as length refers to the length of our input array `prices`.
11. This function returns a list of prices after we've applied a and rounded to the nearest cent, in the form of a list. This is as during function execution, we iterate thorugh each value in the list of prices, apply the discount, round to the nearest cent, then add the new price to our `discounted` list. Then, once iterated through every value, we return the `discounted` list.
12. Given the above object: <br/>
A. student.name <br/>
B. student["Grad Year"] <br/>
C. student.greeting(); <br/>
D. student['Favorite Teacher'].name<br/>
E. student.courseLoad[0]
13. Arithmetic: <br/>
A. String '32', as the 2 gets converted to a string and the strings are concatenated <br/>
B. Number 1, as '3' gets converted to a number then 2 is subtracted <br/>
C. Number 3, as null gets converted to number 0, then 3+0=3 <br/>
D. String '3null', as null is converted to a String 'null', then concatenated with '3' <br/>
E. Number 4, as true gets converted to number 1, then 1+3=4. <br/> 
F. Number 0, as false gets converted to number 0, and null gets converted to number 0, 0+0=0 <br/>
G. String '3undefined', as undefined gets converted to a String 'undefined', then concatenated with '3' <br/>
H. NaN, as undefined gets converted to Number NaN, String '3' gets converted to Number 3, 3 - NaN = NaN
14. Comparison: <br/>
A. True, as String '2' gets converted to Number 2, Number 2 > Number 1 <br/>
B. False, as "lexicographically", the character '2' comes after the character '1', so '2' < '12' <br/>
C. True, as String '2' is converted to Number 2, Number 2 = Number 2. <br/>
D. False, as String '2' and Number 2 are of different types. <br/>
E. False, as Boolean true is converted to Number 1. Number 1 != Number 2.
F. True, as any "non-empty" value for Boolean(x) is true. So Boolean(2) = true, and true === true.
15. The `==` operator will convert values to Numbers if they are of different types, then check equality. The `===` operator does not perform a conversion, and if two values are of different types, we return false, otherwise we check equality.
16. In file `part2-question16.js`.
17. We will return a new array containing elements [2,4,6]. This is as the function `modifyArray` accepts two parameters: `array` and `callback`. Then, `modifyArray`, for each value in `array`, will use the `callback` function on that value, and save the result in an element in `newArr`. Then, we return `newArr`. Basically, we apply a given transformation to a given array, and return our new array. In this case, we multiply each element by 2.
18. In file `part2-question18.js`.
19. The output of the above code is:
```js
1
4
3
2
```
20. 