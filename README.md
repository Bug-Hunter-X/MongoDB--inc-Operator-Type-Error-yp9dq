# MongoDB $inc Operator Type Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numerical field.  However, if the field is not a number or the increment value is not a number, a type error will occur.

## Bug
The original code incorrectly attempts to increment a field with a string value resulting in an error.

## Solution
The corrected code ensures that the field to be incremented is a number and that the increment value is also a number.  Error handling is implemented to gracefully handle cases where the field might not exist.