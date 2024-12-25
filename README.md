# MongoDB $inc operator error with string value
This repository demonstrates a common error in using the MongoDB $inc operator. The error occurs when attempting to increment a field using a string value instead of a numeric value.
## Bug Description
The `$inc` operator in MongoDB is designed to increment a numeric field by a specified value. If you provide a non-numeric value (such as a string), the operation will either fail or produce unexpected results. The code snippet in `bug.js` shows an example of this incorrect usage, using the string '1' instead of the number 1.
## Solution
The corrected code snippet is in `bugSolution.js`. The key change is replacing the string '1' with the number 1. This ensures the `$inc` operator works as intended, correctly incrementing the numeric field.