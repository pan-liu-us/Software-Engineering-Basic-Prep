#### Flipper

```javascript
/*
Flip every pair of characters in a string.

Example:

var input = 'check out how interesting this problem is, it\'s insanely interesting!';
var output = flipPairs(input);
console.log(output); // --> hcce kuo toh wnietertsni ghtsip orlbmei ,si 't sniasenyli tnreseitgn!
*/

function flipPairs(input){
  var flippedInput = "";
  // iterate over the string input, incrementing by 2
  for (var i = 0; i < input.length; i += 2) {
    // check if next character is undefined
    if (input[i + 1] === undefined) {
      // grab currrent character and add to result
      flippedInput += input[i];
      // break - end the for loop
      break;
    }
    // grab next character add to result
    flippedInput += input[i + 1];
    // grab current character and add to the result
    flippedInput += input[i];
  }
  // return result
 return flippedInput;
}

function assertEqual(actual, expected, testName) {
  if (actual === expected) {
    console.log('passed');
  } else {
    console.log ('FAILED [' + testName + '] Expected"' + expected + '", but got"' + actual + '"');
  }
}

var input_1 = 'check out how interesting this problem is, it\'s insanely interesting!';
var actual_1 = flipPairs(input_1);
var expected_1 = "hcce kuo toh wnietertsni ghtsip orlbmei ,si 't sniasenyli tnreseitgn!";

assertEqual(actual_1, expected_1, 'should flip pairs for large sentence with mixed characters');

var input_2 = "abcdef";
var actual_2 = flipPairs(input_2);
var expected_2 = "badcfe";

assertEqual(actual_2, expected_2, 'should flip pairs for small word with only letters');
```

#### Big Flipper

```javascript
/*
Flip every chunk of n characters in a string, where n is any positive integer greater than 1.

Note that this is intentionally very similar to the previous problem.

Please focus on getting a working solution with the tools you know well.

Practice the interactive/collaborative interview style that's described in the documentation.

Example:

var input = 'a short example';
var output = flipEveryNChars(input, 5);
console.log(output); // --> ohs axe trelpma

Breaking this example down piece by piece:

'a sho' -> 'ohs a'
'rt ex' -> 'xe tr'
'ample' -> 'elpma'

-> 'ohs axe trelpma'
*/

function flipEveryNChars(inputString,n) {
  // create a result string
  var flipped = "";
  // split input string into an array, on no delimeter
  var characters = inputString.split("");
  // iterate over the array of characters by n
  for (i = 0; i < characters.length; i += n) {
    // slice the array from current position to current position plus n
    var currentSlice = characters.slice(i, i + n);
    // reservse the array
    var reversedSlice = currentSlice.reverse();
    // join the reversed array
    var joinedSlice = reversedSlice.join("");
    // add resulting string to result
    flipped += joinedSlice;
  }
  // return result
  return flipped;
}

function assertEqual(actual, expected, testName) {
  if (actual === expected) {
    console.log(`passed`);
  } else {
    console.log(`FAILED [${testName}] Expected "${expected}",but got "${actual}"`)
  }
}

var input_1 = 'a short example';
var actual_1 = flipEveryNChars(input_1, 5);
var expected_1 =  'ohs axe trelpma';

assertEqual(actual_1, expected_1, 'should work with input and n is 5');

var input_2 = 'abcdefghijkl';
var actual_2 = flipEveryNChars(input_2, 4);
var expected_2 =  'dcbahgfelkji';

assertEqual(actual_2, expected_2, 'should work with input and n is 4');
```

#### Outliers

```javascript
/*
Given a string of even and odd numbers, find which is the sole even number or the sole odd number.

The return value should be 1-indexed, not 0-indexed.

Examples :
detectOutlierValue("2 4 7 8 10"); // => 3 - Third number is odd, while the rest of the numbers are even
detectOutlierValue("1 10 1 1");  //=> 2 - Second number is even, while the rest of the numbers are odd
*/

function detectOutlierValue(stringOfNums) {
  // split input into an array of stringNums
  var arrayOfStringNums = stringOfNums.split(" ");
  // create arrays for odds and evens
  var odds = [];
  var evens = [];
  // iterate over the array of stringNums
  for (var i = 0; i < arrayOfStringNums.length; i++) {
    // convert current stringNum to a number
    var currentNum = Number(arrayOfStringNums[i]);
    // check if current StringNum is even or odd
      // create an object for that stringNum, with value, and the index (plus 1) where we found it
      // push it to appropirate odds and evens array
    if (currentNum % 2 === 0) {
      evens.push({
        value: currentNum,
        index: i + 1
      })
    } else {
      odds.push({
        value: currentNum,
        index: i + 1
      })
    }  
  }
  // check which array has a length of 1
    // return that array's only value's index value
  if (odds.length === 1) {
    return odds[0].index;
  } else {
    return evens[0].index;
  }
}

function assertEqual(actual, expected, testName) {
  if (actual === expected) {
    console.log(`passed`);
  } else {
    console.log(`FAILED [${testName}] Expected "${expected}",but got "${actual}"`)
  }
}

var actual_1 = detectOutlierValue("2 4 7 8 10");
var expected_1 =  3; //Third number is odd, while the rest of the numbers are even

assertEqual(actual_1, expected_1, 'should work with sole odd number');

var actual_2 = detectOutlierValue("1 10 1 1");
var expected_2 =  2; //Second number is even, while the rest of the numbers are odd

assertEqual(actual_2, expected_2, 'should work with sole even number');
```

#### Transpose

```javascript
/*
You will be given an array that contains two strings. Your job is to create a function that will take those two strings and transpose them, so that the strings go from top to bottom instead of left to right.

e.g. transposeTwoStrings(['Hello','World']);

should return:
H W  
e o  
l r  
l l  
o d
*/

function transposeTwoStrings(arrayInput) {
  // create alias for the first string
  var firstString = arrayInput[0];
  // create alias for the second string
  var secondString = arrayInput[1];
  // create a variable for the longer string
  var longerString;
  // determine longer string
  if ( firstString >= secondString) {
    longerString = firstString;
  } else {
    longerString = secondString;
  }
  // create result string
  var transposedString = "";
  // iterate over length of the lonegr string
    // set first to first string's current letter or empty space
    // set second to second string's current letter or empty space
    // add first, space, second, and newline to the result string
  for (var i = 0; i < longerString.length; i++) {
    var firstCharacter = firstString[i] || " ";
    var secondCharacter = secondString[i] || " ";
    transposedString += firstCharacter + " " + secondCharacter + "\n";

  }
  // return result string
  return transposedString;
}

console.log(transposeTwoStrings(['Hello','World']));
console.log("\n");
console.log(transposeTwoStrings(['some','thing']));
```

#### Find the Pair

```javascript
/*
Given a list of non-negative integers and a target sum, find a pair of numbers that sums to the target sum.

Example:

var pair = findPairForSum([3, 34, 4, 12, 5, 2], 9);
console.log(pair); // --> [4, 5]

*/

function findPairForSum(integers, targetSum) {
  //create a result array
  var pair = [];
  // iterate over the outer integers
  for (var j = 0; j < integers.length - 1; j++) {
    // iterate from current integer over rest of intengers
    for ( var k = j + 1; k < integers.length; k++) {
      // check sum
      if (integers[j] + integers[k] === targetSum) {
        // push to the result array
        pair.push(integers[j], integers[k]);
      }
    }
  }
  // return result array
  return pair;
}

function assertArrayEqual(actual, expected, testName) {
  var sameLength = actual.length === expected.length;
  var sameValue = true;
  for (var i = 0; i < expected.length; i++) {
    if (expected[i] !== actual[i]) {
      sameValue = false;
      break;
    }
  }

  if (sameLength && sameValue) {
    console.log(`passed`);
  } else {
    console.log(`FAILED [${testName}] Expected ${expected}, but got ${actual}`);
  }
}

var actualFound = findPairForSum([3, 34, 4, 12, 5, 2], 9);
var expectedFound = [4,5]
assertArrayEqual(actualFound, expectedFound, 'should return an array of the two integers that sum to target')

var actualNotFound = findPairForSum([3, 34, 4, 12, 5, 2], 11);
var expectedNotFound = []
assertArrayEqual(actualNotFound, expectedNotFound, 'should return an empty array wehn sum cannot be made')
```

#### Rotate This

```javascript
/*
Is one string a rotated version of another?

For example:
String 1: 'hello world'
String 2: 'orldhello w'

Extra hint: 
If you double the string, you'll be able to find another string inside the doubled string using familiar String methods.

Doubled string: 'hello worldhello world'
Search w/in it: '       orldhello w    '
*/

function isRotated(str1, str2) {
  // cretae doubled version of str1
  var doubled = str1 + str1;
  // check for indexOf str2  with double str1
  var index = doubled.indexOf(str2);
  // if present
      // return ture
      // otherwise
    // return false
  if (index !== -1) {
    return true;
  } else {
    return false;
  } 
}


function assertEqual(actual, expected, testName) {
  if (actual === expected) {
    console.log(`passed`);
  } else {
    console.log(`FAILED [${testName}] Expected ${expected}, but got ${actual}`)
  }
}

var actualRotate = isRotated('hello world','orldhello w');
var expectedRotate = true;
assertEqual(actualRotate, expectedRotate, 'should return true when string 2 is rotated version of string 1')

var actualNot = isRotated('hellow world','orldhello w');
var expectedNot = false;
assertEqual(actualNot, expectedNot, 'should return false when string 2 is not rotated version of string 1')
```

#### Divide and Conquer

```javascript
/*
Binary search is a technique for very rapidly searching a sorted collection by cutting the search space in half at every pass.

Given a sorted array, such as this:
[1, 3, 16, 22, 31, 33, 34]

You can search for the value 31, as follows:

1) Pick the midpoint: 22.
2) The value is higher than 22, so now consider only the right half of the previous array:
[...31, 33, 34]
3) Pick the midpoint: 33
4) The value is lower than 33, so now consider only the left half of the previous array:
[...31...]
5) Pick the midpoint: 31
6) You've hit the value.
7) Return the index of the value.

Notes:
* If you don't find the value, you can return null.
* If at any point you calculate the index of the midpoint and get a fractional number, just round it down ("floor" it).
*/

function binarySearch (array,target) {
  var min = 0;
  var max = array.length - 1;
  var midpoint = Math.floor((min + max) / 2);

  while (min <= max) {
    if (target === array[midpoint]) {
      return midpoint;
    }
    // if target is less than the value at the midpoint
    if (target < array[midpoint]) {
      // reset max to be midpoint - 1
      max = midpoint - 1;
    }

    // if target is greater than the value at the midpoint
    if (target > array[midpoint]) {
      // reset min to be midpont + 1
      min = midpoint + 1;
    }

    // re-guess or reset midpoint to be middle of the remaining array
    midpoint = Math.floor((min + max) / 2);
  }

  // if while loop is stops, we know the target value is Not present

return null;

}

function assertEqual (actual,expected,testName) {
  if (actual === expected) {
    console.log(`passed`)
  } else {
    console.log(`FAILED [${testName}] Expected "${expected}", but got "${actual}""`)
  }
}

var actualFound = binarySearch([1, 3, 16, 22, 31, 33, 34],31);
var expectedFound = 4;
assertEqual(actualFound,expectedFound,'should return index of value when value is present')

var actualNotFound = binarySearch([1, 3, 16, 22, 31, 33, 34],9);
var expectedNotFound = null;
assertEqual(actualNotFound,expectedNotFound,'should return null when value is not present')
```
