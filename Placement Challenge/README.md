## Basics

#### Create a string

Declare a variable, call it myString, and assign it to any string of your choosing.

(Hint: You do not need to write anything other than the described statement.)

```javascript
// on the line below, declare a variable named myString,
// then assign it to any string of your choosing
var myString = "hello";
```

#### Create an Array

Declare a variable, call it myArray, and assign it to any array containing three elements. The elements can be of any type.

(Hint: You do not need to write anything other than the described statement.)

```javascript
// on the line below, declare a variable named myArray,
// then assign it to an array with 3 elements
var myArray = [0, false, null];
```

#### Create an Object
Submitted on Today at 3:54 PM
Declare a variable, call it myObject, and assign it to an object literal with 3 properties.

(Hint: You do not need to write anything other than the described statement.)

```javascript
// on the line below, declare a variable named myObject,
// then assign it to an object literal with 3 properties
var myObject = {key: "value", num: 0, bool:true};
```

#### Concatenate Two Strings

Complete the function concatenateTwoStrings. This function will take in two string parameters, and should return a string which is the result of concatenating the two input strings together.

```javascript
var output = concatenateTwoStrings("stair", "case");
console.log(output); // "staircase"
```

```javascript
function concatenateTwoStrings(string1, string2) {
  return string1 + string2;
}
```

#### String Interpolation

Complete the function 'interpolate'. This function will take in a string parameter, and return a string as follows:

```javascript
var message1 = interpolate("turkey");
console.log(message1); // "My favorite food is turkey!"

var message2 = interpolate("tofurkey");
console.log(message2); // "My favorite food is tofurkey!"
Pay close attention to the punctuation in the resulting string.
```

```javascript
function interpolate(favoriteFood) {
  return `My favorite food is ${favoriteFood}!`;
}
```

#### indexOf on a String
Submitted on Today at 3:56 PM
Complete the function indexOfString. This function will take in two string parameters, and return the index, inside of the first string, where the second string is located. You will want to use the indexOf method for Strings. If string2 is not present within string1, your function should return -1.

```javascript
var output = indexOfString("environment", "iron");
console.log(output); // 3
```

```javascript
function indexOfString(string1, string2) {
  // it returns the correct index when string2 is present within string1
  // it returns -1 when string2 is not present within string1
  return string1.indexOf(string2);
}
```

#### Split a String

Complete the function splitString. This function will take in one parameter, a string to be split, and should return an array that is the result of calling the split method on the input string. You should call split with an argument of an empty string. You will want to use the split method for Strings.

```javascript
var output = splitAString("queue");
console.log(output); // ["q", "u", "e", "u", "e"]
```

```javascript
function splitAString(str) {
  // it splits the input string on an empty string
  return str.split("");
}
```

#### Remove element from back of an Array

Complete a function called removeFromBack. Given an array, removeFromBack returns the input array with its last element removed. You should be familiar with the Array method pop.

```javascript
var output = removeFromBack([1, 2, 3]);
console.log(output); // --> [1, 2]
```

```javascript
function removeFromBack(arr) {
  // it should remove the last element from an array and handle an empty array
  arr.pop();
  return arr;
}
```

#### Add element to end of an Array

Complete a function called addToBack. Given an array and an element of any type, addToBack adds the input element to the back of the input array, and returns the input array. Your function should return the INPUT array, rather than create a new one. You should be familiar with the Array method push.

```javascript
var output = addToBack([1, 2], 3);
console.log(output); // -> [1, 2, 3]
```

```javascript
function addToBack(arr, element) {
  // it should add an element to the end of an array or empty array and should be the same array instance that was passed in
  arr.push(element);
  return arr;
}
```

#### Remove an element from beginning of an Array

Complete a function called removeFromFront. Given an array, removeFromFront returns the input array with its first element removed. You should be familiar with the Array method shift.

```javascript
var output = removeFromFront([1, 2, 3]);
console.log(output); // --> [2, 3]
```

```javascript
function removeFromFront(arr) {
  // it should return the array with the first element removed and should handle an empty array
  arr.shift();
  return arr;
}
```

#### Add an element to beginning of an Array

Complete a function called addToFront. Given an array and an element of any type, addToFront adds the input element to the front of the input array, and returns the input array. Your function should return the INPUT array, rather than create a new one. You should be familiar with the unshift method.

```javascript
var output = addToFront([1, 2], 3);
console.log(output); // -> [3, 1, 2]
```

```javascript
function addToFront(arr, element) {
  // it should add an element to the beginning of an array or empty array and should be the same array instance that was passed in
  arr.unshift(element);
  return arr;
}
```

#### Using slice

We are going to complete a function that takes in three parameters, an array and two integer indexes. Your function should apply the slice method to the input array, from the first integer index to the last integer index, and return the result of this operation.

```javascript
function useSlice(array, start, end) {
  // it applies slice to input array from start (is defined) to end and returns the results with no index arguments are passed in
  return array.slice(start, end);
}
```

#### Using Splice

Complete a function that demonstrates how to use the splice method on an array. usingSplice will take 4 parameters, an array, an integer start, an integer deleteCount, and a String item. Your function should splice the input array: starting at the input start, deleting deleteCount items, and inserting item into the array at start. Your function need not return anything.

```javascript
function usingSplice(array, start, deleteCount, item) {
  // it removes "deleteCount" elements from index "start", and inserts "item"
  return array.splice(start, deleteCount, item);
}
```

#### indexOf on an Array

Complete the function indexOfArray. This function will take in two parameters, an array and an element, and returns the index, inside of the array, where the element is located. You will want to use the indexOf method for Arrays. If the element is not present within array, your function should return -1.







