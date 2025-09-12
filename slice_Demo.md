
###  Topic: Array Slice Example

####  Question  
What will be the output of the following JS code?

```javascript
const proPeersArr = [1, 2, 3, 4, 5];
const proPeersSlice = proPeersArr.slice(1, 3);
console.log(proPeersSlice);
ans => 2,3

slice(start, end) returns a shallow copy of the array from the start index up to but not including the end index.

 # slice(start, end)

Does not modify the original array.
Returns a new array containing the selected elements.
End index is exclusive.
splice(start, deleteCount, ...items)
Modifies the original array.
Can remove or add elements.


