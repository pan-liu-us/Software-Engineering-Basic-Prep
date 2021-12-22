## Testing

#### assertEqual

```javascript
//assertEqual
function assertEqual(actual,expected,testName){
    if (actual === expected) {
        console.log(`passed`);
    } else {
        console.log(`FAILED [${testName}] Expected "${expected}", but got "${actual}"`);
    }
}

//SUCCESS CASE
function multiplyByTwo(n) {
  return n * 2;
}
var output = multiplyByTwo(2); // returns 4
assertEqual(output, 4, 'it doubles 2 to 4');
// console output:
// passed


//FAILURE CASE
function multiplyByTwo(n) {
  return (n * 2) + 1; // an incorrect implementation
}
var output = multiplyByTwo(2); // returns 5
assertEqual(output, 4, 'it doubles 2 to 4');
// console output:
// FAILED [it doubles 2 to 4] Expected "4", but got "5"
```

#### assertArraysEqual

```javascript
//assertArraysEqual
function assertArraysEqual(actual, expected, testName) {
    var areEqualLength = actual.length === expected.length;
    var areEqualItems = true;
    for (var i = 0; i < expected.length; i++) {
        if (expected[i] !== actual[i]) {
            areEqualItems = false;
            break;
        }
    }
    if (areEqualLength && areEqualItems) {
        console.log(`passed`);
    } else {
        console.log(`FAILED [${testName}] Expected "${expected}", but got "${actual}"`);
    } 
}

//SUCCESS CASE
var expected = ['b', 'r', 'o', 'k', 'e', 'n'];
var actual = 'broken'.split('');
assertArraysEqual(actual, expected, 'splits string into array of characters');
// console output:
// passed

//FAILURE CASE
var expected = [1, 1, 2, 3, 5, 8, 13];
var actual = generateFirstNFibonaccis(7);
assertArraysEqual(actual, expected, 'generates first 7 Fibonacci numbers');
// console output:
// FAILED [generates first 7 Fibonacci numbers] Expected "1, 1, 2, 3, 5, 8, 13", but got "2, 3, 5, 8, 13, 21, 34"
```

PS: CORRECT generateFirstNFibonaccis function:

```javascript
function generateFirstNFibonaccis(n) {
    if (n === 2) {
        return [1, 1];
    } else {
        var s = generateFirstNFibonaccis(n - 1);
        s.push(s[s.length - 1] + s[s.length - 2]);
        return s;
    } 
}
```

#### assertObjectsEqual

```javascript
function assertObjectsEqual(actual, expected, testName) {
    actual = JSON.stringify(actual);
    expected = JSON.stringify(expected);
    if (actual === expected) {
        console.log('passed');
    } else {
        console.log(`FAILED [${testName}] Expected ${expected}, but got ${actual}`);
    }
}

//SUCCESS CASE:
var person = {
  firstName: 'Cassidy',
  lastName: 'Jacobs'
};
updateObject(person, 'firstName', 'Jack');

var expected = {
  firstName: 'Jack',
  lastName: 'Jacobs'
};

assertObjectsEqual(person, expected, "updates person's existing first name field");
// console output:
// passed

//FAILURE CASE (We will assume that updateObject does NOT work):
var person = {
  firstName: 'Joe',
  lastName: 'Blow'
};
updateObject(person, 'age', 35);

var expected = {
  firstName: 'Joe',
  lastName: 'Blow',
  age: 35
};
assertObjectsEqual(person, expected, "adds person's non-existing age field");
// console output:
// FAILED [adds person's non-existing age field] Expected {"firstName":"Joe", "lastName":"Blow", age:35}, but got {"firstName":"Joe", "lastName":"Blow"}
```



#### assertWithinRange

```javascript
function assertWithinRange(low, high, actual, testName) {
    var inRange = (low <= actual) && (actual <= high);
    if (inRange) {
        console.log('passed');
    } else {
        console.log('FAIL [' + testName + '] "' + actual + '" not within range ' + low + ' to ' + high);
    }
}

//SUCCESS CASE:
var blackjackScore = 20;
assertWithinRange(4, 21, blackjackScore, 'blackjack score should be between 4 and 21');
// console output:
// passed

//SUCCESS CASE:
var dieRoll = 1;
assertWithinRange(1, 6, dieRoll, 'die roll should be between 1 and 6');
// console output:
// passed

//FAILURE CASE:
var price = 101;
assertWithinRange(1, 100, price, 'price should be between 1 and 100');
// console output:
// FAIL [price should be between 1 and 100] "101" not within range 1 to 100
```

#### Sample of Clean Code Structure

```javascript
// FUNCTION DEFINITION(S)
function addOne(val) {
  return val + 1;
}

// ASSERTION FUNCTION(S) TO BE USED
function assert(condition, testName) {
  if (condition) {
    console.log('passed');
  } else {
    console.log('FAILED [' + testName + ']');
  }
}

// TESTS FOR isOne
var result1 = addOne(1);
assert(result1 === 2, 'should return result of a positive input number added to 1');

var result2 = addOne(-2);
assert(result2 === 1, 'should return result of a negative input number added to 1');
```

#### Applying assertEqual 1

```javascript
// FUNCTION DEFINITION(S)
function square(n) {
    return n * n;
}

// ASSERTION FUNCTION(S) TO BE USED
function assertEqual(actual,expected,testName){
    if (actual === expected) {
        console.log('passed');
    } else {
        console.log('FAILED [' + testName + '] Expected "' + expected + '", but got "' + actual + '"');
    }
}

// TESTS CASES
assertEqual(square(3), 9, 'it should square a positive integer');
```

#### Applying assertEqual 2

```javascript
// Note: This is a simple, albeit temporarily incorrect implementation of the standard Array method "every()":
// https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Array/every

// FUNCTION DEFINITION
function every(array, callbackFunction) {
    var doesEveryElementMatch = true;
    for (var i = 0; i < array.length; i++) {
        if (doesEveryElementMatch === false) {
            break;
        }
        doesEveryElementMatch = callbackFunction(array[i]);
    }
    return doesEveryElementMatch;
}

// ASSERTION FUNCTION(S) TO BE USED
function assertEqual(actual, expected, testName) {
    if (actual === expected) {
        console.log('passed');
    } else {
        console.log('FAILED [' + testName + '] Expected "' + expected + '", but got "' + actual + '"');
    }
}

function isLessThan10(num) {
    return num < 10;
}

var sampleArrayTrue = [1, 4, 9];
var actualTrue = every(sampleArrayTrue, isLessThan10);
var expectedTrue = true;
assertEqual(actualTrue, expectedTrue, 'should return true when all elements pass the test function');

var sampleArrayFalse = [1, 11, 9];
var actualFalse = every(sampleArrayFalse, isLessThan10);
var expectedFalse = false;
assertEqual(actualFalse, expectedFalse, 'should return false when at least one element does not pass the test function');
```

#### Applying assertArraysEqual

```javascript
// FUNCTION DEFINITIONS
function map(array, callbackFunction) {
    var newArray = [];
    for (var i = 0; i < array.length; i++) {
    newArray.push(callbackFunction(array[i]));
  }
    return newArray;
}

function cubeAll(numbers) {
    return map(numbers, function(n) {
    return n * n * n;
    });
}

// ASSERTION FUNCTION(S) TO BE USED
function assertArraysEqual(actual, expected, testName) {
    var areEqualLength = actual.length === expected.length;
    var areEqualItems = true;
    for (var i = 0; i < expected.length; i++) {
        if (expected[i] !== actual[i]) {
        areEqualItems = false;
        break;
        }
    }

    if (areEqualLength && areEqualItems) {
        console.log('passed');
    } else {
        console.log('FAILED [' + testName + '] Expected "' + expected + '", but got "' + actual + '"');
    }
}

// TESTS FOR MAP
function doubleElement(num) {
    return num * 2;
}

var mapTestArray = [1, 2, 3, 4];
var actualMapTest = map(mapTestArray, doubleElement);
var expectedMapTest = [2, 4, 6, 8];
assertArraysEqual(actualMapTest, expectedMapTest, 'should apply callbackFunction to each element and return results in an array');

// TESTS FOR CUBE ALL

var cubeAllTestArray = [1, 2, 3, 4];
var actualCubeAllTest = cubeAll(cubeAllTestArray);
var expectedCubeAllTest = [1, 8, 27, 64];
assertArraysEqual(actualCubeAllTest, expectedCubeAllTest, 'should cube all elements and return results in an array');
```

#### Applying assertObjectsEqual

```javascript
// FUNCTION DEFINITION
function addFullNameProp(obj) {
  var firstName = obj['firstName'];
  var lastName = obj['lastName'];

  if (firstName && lastName) {
    obj['fullName'] = firstName + ' ' + lastName;
  }

  return obj;
}

// ASSERTION FUNCTION(S) TO BE USED
function assertObjectsEqual(actual, expected, testName) {
  actual = JSON.stringify(actual);
  expected = JSON.stringify(expected);

  if ( actual === expected ) {
    console.log('passed');
  } else {
    console.log('FAILED [' + testName + '], expected "' + expected + '", but got "' + actual + '"')
  }
}

// TESTS FOR ADD FULL NAME PROP
var person = {
  firstName: 'Chris',
  lastName: 'Riccolo'
};
var actualResult1 = addFullNameProp(person);
var expectedResult1 = {
  firstName: 'Chris',
  lastName: 'Riccolo',
  fullName: 'Chris Riccolo'
};
assertObjectsEqual(actualResult1, expectedResult1, 'should add fullName property when firstName and lastName are defined');

var missingValues1 = {
  firstName: 'Chris'
};
var actualMissing1 = addFullNameProp(missingValues1);
var expectedMissing1 = {
  firstName: 'Chris'
};
assertObjectsEqual(actualMissing1, expectedMissing1, 'should not add fullName property when lastName is undefined');

var missingValues2 = {
  lastName: 'Riccolo'
};
var actualMissing2 = addFullNameProp(missingValues2);
var expectedMissing2 = {
  lastName: 'Riccolo'
};
assertObjectsEqual(actualMissing2, expectedMissing2, 'should not add fullName property when firstName is undefined');
```

## Skeletons

```javascript
// FUNCTION DEFINITION
function addFullNameProp(obj) {
  // set variable equal to firstName property within input object
  // set variable equal to lastName property within input object
  // if firstName and lastName are both defined
    // add a property to input object - key: fullName, value firstName and lastName with space in between

  // return input object
}

// ASSERTION FUNCTION(S) TO BE USED
function assertObjectsEqual(actual, expected, testName) {
  // Write assertObjectsEqual because function returns an object
}

// TESTS FOR ADD FULL NAME PROP
// Test object with both first and last name is defined in input object
// Test object with last name missing
// Test object with first name missing
```

#### Average

```javascript
// FUNCTION DEFINITION(S)
function sum(numbers) {
  // returns the sum of an array of numbers
  var result = 0;
  for (var i = 0; i < numbers.length; i++){
      result += numbers[i]
  }
  return result;
}


function average(numbers) {
  // uses sum function
  // returns the average of an array of numbers
    return sum(numbers) / numbers.length;
}


// ASSERTION FUNCTION(S) TO BE USED
function assertEqual(actual, expected, testName) {
  if (actual === expected) {
    console.log('PASSED [' + testName + ']');
  } else {
    console.log('FAILED [' + testName + '] Expected "' + expected + '", but got "' + actual + '"');
  }
}

// TESTS CASES
var input = [1,2,3,4,5];

// TESTS FOR SUM
var actualSumResult = sum(input);
var expectedSumResult = 5;
assertEqual(actualSumResult, expectedSumResult, 'should accurately sum the integers in an array');

///TEST FOR AVERAGE
var actualAverageResult = average(input);
var expectedAverageResult = 3;
assertEqual(actualAverageResult, expectedAverageResult, 'should accurately calculate the average of integers in an array');
```

#### Decorate Student List

```javascript
// FUNCTION DEFINITIONS
function getRandomIntInclusive(min, max) {
    min = Math.ceil(min);
    max = Math.floor(max);
    return Math.floor(Math.random() * (max - min + 1)) + min;
}

function decorateClassListWithAges(classList) {
    // creates an object for each string in the input array, with an age of 10 or 11
    // returns an array of these objects
    var decoratedClassList=[];
    for (var i=0;i<classList.length;i++){
        var currentStudent = {};
        currentStudent.name = classList[i];
        currentStudent.age = getRandomIntInclusive(10,11);
        decoratedClassList.push(currentStudent);
    }
    return decoratedClassList;
}

// ASSERTION FUNCTION(S) TO BE USED
function assertWithinRange(low, high, actual) {
    if(low <=actual && actual <= high){
    return true;
    } else {
        return false;
    }
}

function testDecoratedStudentList(input,output){
    for (var j = 0; j < input.length;j ++) {
        if (input[j]!==output[j].name) {
            console.log('FAILED: Incorrect name at index:' + j);
        return;
        }
        if (assertWithinRange(10,11,output[j].age) === false) {
            console.log('FAILED: Incorrect age at index:' + j);
        return;
        }
    }
console.log('passed');
}


// TESTS FOR DECORATE STUDENT LIST

var classList = ["Joe", "Jack", "John", "Fred", "Frank", "Barry", "Larry", "Mary",
  "Harry", "Farrell", "Susan", "Monica", "Keira", "Caroline", "Harriet", "Erica",
  "Luann", "Cheryl", "Beth", "Rupa", "Linda", "Allison", "Nancy", "Dora"];

var decoratedList = decorateClassListWithAges(classList);

testDecoratedStudentList(classList,decoratedList);
```

#### Isograms

Notes:

- Assume your input is only letters.
- Assume the empty string is an isogram.
- Ignore case.
- Follow the pseudocode exactly!

```javascript
// FUNCTION DEFINITION(S)
function isIsogram(text) {
    // add each char to a set
    // https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set
    // note: a set drops dup values
    // thus, to see if all the chars were unique,
    // check length of text and the size of the set
    text = text.toLowerCase();
    var letters = text.split('');
    letters = new Set(letters);
    return text.length === letters.size;
}

// ASSERTION FUNCTION(S) TO BE USED
function assertEqual(actual, expected, testName){
    if (actual === expected){
        console.log('passed');
    } else { 
        console.log('FAILED [' + testName +'] Expected + "'+ expected + '" but got"' + actual +'"');
    }    
}

// TESTS CASES
assertEqual(isIsogram(''), true, 'should return true for an empty string');
assertEqual(isIsogram('true'), true, 'should return true for an isogram');
assertEqual(isIsogram('assert'), false, 'should return false for non-isogram');
assertEqual(isIsogram('caCAtcHh'), false, 'should ignore case');
```

#### Interpret A Skeleton

```javascript
// FUNCTION DEFINITION(S)
function findMaxRepeatCountInWord(word) {
    // Break up individual word into individual letters.
    // Count the instances of each letter
    // Iterate all the counts and find the highest
    // Return this word's max repeat count
    var letters = word.split('');
    var letterCount = {};
    for (var i = 0; i < letters.length; i++) {
        var currentLetter = letters[i];
        if (letterCount[currentLetter] === undefined) {
            letterCount[currentLetter] = 1;
        } else {
            letterCount[currentLetter]+=1
        }
    }
  
    var max = 0;
    for (letter in letterCount) {
        if (letterCount[letter] > max) {
        max = letterCount[letter];
        }
    }
  
    return max;
}


function findFirstWordWithMostRepeatedChars(text) {
    var maxRepeatCountOverall = 0;
    var wordWithMaxRepeatCount = '';

    // Break up input text into words (space-delimited).
    // For each word...
    var words = text.split(' ');
    for (var j = 0; j < words.length; j++) {
        var repeatCountForWord = findMaxRepeatCountInWord(words[j]);
        // If that max repeat count is higher than the overall max repeat count, then
            // update maxRepeatCountOverall
         // update wordWithMaxRepeatCount
        if (repeatCountForWord > maxRepeatCountOverall) {
            maxRepeatCountOverall = repeatCountForWord;
            wordWithMaxRepeatCount = words[j];
        }
    }
  return wordWithMaxRepeatCount;
}

// ASSERTION FUNCTION(S) TO BE USED
function assertEqual(actual, expected, testName) {
    if (actual === expected) {
        console.log('passed');
    } else {
        console.log('FAILED [' + testName + '] Expected "' + expected + '", but got "' + actual + '"');
    }
}


// TESTS CASES
// TESTS FOR findMaxRepeatCountInWord
var actualMaxCount = findMaxRepeatCountInWord('bananas');
var expectedMaxCount = 3;
assertEqual(actualMaxCount, expectedMaxCount, 'should return count of letter that is repeated most often in input word');

// TESTS FOR findFirstWordWithMostRepeatedChars
var actualWord = findFirstWordWithMostRepeatedChars('bananas are excellent');
var expectedWord = 'bananas';
assertEqual(actualWord, expectedWord, 'should return word with most repeated letters');
```

#### Render Phone Number (Optional)

```javascript
// FUNCTION DEFINITION(S)
function PhoneNumberFormatter(numbers) {
  this.numbers = numbers;
}

PhoneNumberFormatter.prototype.render = function() {
  var string = '';
  string += this.parenthesize(this.getAreaCode());
  string += ' ';
  string += this.getExchangeCode();
  string += '-';
  string += this.getLineNumber(); 
  return string;
};

PhoneNumberFormatter.prototype.getAreaCode = function() {
  return this.slice(0,3);
};

PhoneNumberFormatter.prototype.getExchangeCode = function() {
  return this.slice(3,6);
};

PhoneNumberFormatter.prototype.getLineNumber = function() {
  return this.slice(6,10);
};

PhoneNumberFormatter.prototype.parenthesize = function(string) {
  return '(' + string + ')';
};

PhoneNumberFormatter.prototype.slice = function(start, end) {
  return this.numbers.slice(start, end).join('');
};

// ASSERTION FUNCTION(S) TO BE USED
function assertEqual(actual, expected, testName) {
  if (actual !== expected) {
    console.log('FAILED [' + testName + '] Expected "' + expected + '", but got "' + actual + '"');
  } else {
    console.log('PASSED [' + testName + ']');
  }
}


// TESTS CASES
var formatter = new PhoneNumberFormatter([6, 5, 0, 8, 3, 5, 9, 1, 7, 2]);
assertEqual(formatter.render(), '(650) 835-9172', 'should render phone number in correct format');
```

#### Find Longest Palindrome

Similarly to some of the previous problems in this section, there is a concept here that will be new to you. Ideally, your solution will use a native method (built into the language) called .sort(). Essentially, when called, this method takes a function that tells the sorting operation how it should order the resulting sorted array. We have supplied a function inside of the skeleton. Please consult this MDN documentation, and read it carefully: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort 

```javascript
// FUNCTION DEFINITIONS
function findLongestPalindrome(sentence) {
    var words = sentence.split(' ');
    var palindromes = [];
    for (var i = 0; i < words.length; i++) {
        if (isPalindrome(words[i])) {
            palindromes.push(words[i]);  
        }
    }
    sortedPalindromes = palindromes.sort(sortAscendingByLength); 
    var longestPalindrome = sortedPalindromes.pop();
    return longestPalindrome;
}

function reverseString(string) {
    var splitString = string.split('');
    var reversedSplitString = splitString.reverse();
    var reversedString = reversedSplitString.join('');
    return reversedString;
}

function isPalindrome(word) {
    word = word.toLowerCase();
    return word === reverseString(word);
}

function sortAscendingByLength(a, b) {
    if (a.length > b.length) {
        return 1;
    } else if (a.length < b.length) {
        return -1;
    } 
    return 0;
}

// ASSERTION FUNCTION(S) TO BE USED
function assertEqual(actual, expected, testName) {
    if (actual === expected) {
        console.log('passed');
    } else {
        console.log('FAILED [' + testName + '] Expected "' + expected + '", but got "' + actual + '"');
    }
}

function assertArraysEqual(actual, expected, testName) {
    var areEqualLength = actual.length === expected.length;
    var areEqualItems = true;
    for (var i = 0; i < expected.length; i++) {
        if (expected[i] !== actual[i]) {
            areEqualItems = false;
            break;
        }
    }
    if (areEqualLength && areEqualItems) {
        console.log('passed');
    } else {
        console.log('FAILED [' + testName + '] Expected "' + expected + '", but got "' + actual + '"');
    }
}

// TESTS FOR SORT ASCENDING BY LENGTH
var unsortedStringsArray = ['little', 'small', 'a', 'base', 'trapeze'];
var actualSorted = unsortedStringsArray.sort(sortAscendingByLength);
var expectedSorted = ['a', 'base', 'small', 'little', 'trapeze'];

assertArraysEqual(actualSorted, expectedSorted, 'should sort an array of strings into ascending order by length');

// TESTS FOR REVERSE STRING
var inputString = 'medicine';
var actualReversed = reverseString(inputString);
var expectedReverse = 'enicidem';

assertEqual(actualReversed, expectedReverse, 'should return an input string reversed');

// TESTS FOR IS PALINDROME
var palindrome = 'racecar';
var actualResult = isPalindrome(palindrome);
var expectedResult = true;

assertEqual(actualResult, expectedResult, 'should return true for a valid palindrome');

// TESTS FOR FIND LONGEST PALINDROME
var sentence = 'alula ana hannah madam minim';
var actualLongest = findLongestPalindrome(sentence);
var expectedLongest = 'hannah';

assertEqual(actualLongest, expectedLongest, 'should return the longest palindrome in an input sentence');
```

## Fashion Inventory Problems

### Part A
### Part B
### Part C
### Part D
