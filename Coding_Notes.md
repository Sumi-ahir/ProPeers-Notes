 # Question

+ Which command in Unix is used to display the current directory's contents?
  ANS :ls

#  Identify the mistake in this command:

+ db.collection.createIndex({ age: "-1" })

  ANS :Incorrect index type

Explanation

In MongoDB, when creating an index, the sort order must be a number (1 for ascending, -1 for descending).

In the given code, " -1 " is written as a string instead of a number.

Correct syntax should be:

db.collection.createIndex({ age: -1 }) 


That’s why the error is → Incorrect index type.
