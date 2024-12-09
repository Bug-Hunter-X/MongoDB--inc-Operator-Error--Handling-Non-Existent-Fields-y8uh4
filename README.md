# MongoDB $inc Operator Error: Handling Non-Existent Fields

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numerical field by a specified value.  However, if the field does not exist, the operation may fail silently or produce unexpected results.

The `bug.js` file shows an incorrect implementation that can lead to errors.  The `bugSolution.js` file demonstrates the correct approach using the `upsert` option to handle cases where the field may not exist.

## How to Reproduce the Bug

1.  Ensure you have a MongoDB instance running.
2.  Clone this repository.
3.  Run `bug.js`.  Observe the potential error or unexpected behavior if the 'likes' field is not present.
4. Run `bugSolution.js` to see how the `upsert` option solves this issue.
