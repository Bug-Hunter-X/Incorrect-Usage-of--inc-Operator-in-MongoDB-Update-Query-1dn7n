# Incorrect Usage of $inc Operator in MongoDB Update Query
This example demonstrates an incorrect usage of the `$inc` operator in a MongoDB update query. The `$inc` operator is used to increment or decrement a numeric value in a document.  Attempting to increment a field with a non-numeric value will result in an error.

## Bug
The provided code attempts to increment the `field` in a document with the value 'string', which is not a number.  This will produce an error because `$inc` expects a numeric value.

## Solution
The solution replaces the string value with an appropriate number. 
