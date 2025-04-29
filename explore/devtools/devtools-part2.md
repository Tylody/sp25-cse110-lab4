# DevTools - Part 2
1. The bug was that our inputs are of type string, so when we do `num1 + num2`, it does a string concatenation operation rather than an arithmetic addition operation.
2. I would fix it by wrapping our inputs in `parseFloat()`, so that the values are converted to numbers, therefore being added as nubmers. (check `fix.png`)