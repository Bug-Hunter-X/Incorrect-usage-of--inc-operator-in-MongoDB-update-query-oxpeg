# Incorrect usage of $inc operator in MongoDB update query
This repository demonstrates an uncommon error in MongoDB when using the $inc operator in update queries. The error arises from providing a string value instead of a numerical value to the $inc operator.

## Bug
The bug lies in the incorrect usage of the $inc operator within a MongoDB update query.  Instead of incrementing the 'count' field by 1, the query adds a new field with the name "1" and the value "1".

## Solution
The solution is straightforward and involves ensuring that the value provided to the $inc operator is a number (integer or float).

## How to reproduce the bug
1. Clone this repository.
2. Make sure you have MongoDB set up and running.
3. Run `bug.js` . Observe the result.
4. Run `bugSolution.js` and observe the correct result.