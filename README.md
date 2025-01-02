# MongoDB $inc operator with string value
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator requires a numeric value for the increment. Using a string will lead to unexpected behavior or an error. The solution shows the correct way to use `$inc` with a numeric value.

## Bug
The bug is caused by passing a string value ("1") instead of a numeric value (1) to the `$inc` operator in the `updateOne` method. This results in an update failure or unexpected results.

## Solution
The solution provides a corrected version where a numeric value (1) is used to increment the `age` field, ensuring the update operation executes as expected.