Conditionals 1 - 9
Objects 1 - 13
String Methods 1 - 3
Math 1- 6
Array Methods 1 - 16
Array String Methods 1 - 2
Advanced 1 - 8
Interation 1 - 6
Convert Array To Object 1 - 3
Convert Object To Array 1 - 3

## Conditionals 1 - 9

### Conditionals 1

#### isOldEnoughToDrink

Write a function called "isOldEnoughToDrink". Given a number, in this case an age, "isOldEnoughToDrink" returns whether a person of this given age is old enough to legally drink in the United States. Notes:

- The legal drinking age in the United States is 21.

```javascript
var output = isOldEnoughToDrink(22);
console.log(output); // --> true
```

```javascript
function isOldEnoughToDrink(age) {
  if (age >= 21) {
      return true;
  } else {
      return false;
  }
}
```

#### isOldEnoughToDrive

Write a function called "isOldEnoughToDrive". Given a number, in this case an age, "isOldEnoughToDrive" returns whether a person of this given age is old enough to legally drive in the United States. Notes:

- The legal driving age in the United States is 16.

```javascript
var output = isOldEnoughToDrive(22);
console.log(output); // --> true
```

```javascript
function isOldEnoughToDrive(age) {
    if (age >= 16) {
      return true;
  } else {
      return false;
  }
}
```

#### isOldEnoughToVote

Write a function called "isOldEnoughToVote". Given a number, in this case an age, 'isOldEnoughToVote' returns whether a person of this given age is old enough to legally vote in the United States. Notes:

- The legal voting age in the United States is 18.

```javascript
var output = isOldEnoughToVote(22);
console.log(output); // --> true
```

```javascript
function isOldEnoughToVote(age) {
    if (age >= 18) {
      return true;
  } else {
      return false;
  }
}
```

#### isOldEnoughToDrinkAndDrive

Write a function called "isOldEnoughToDrinkAndDrive". Given a number, in this case an age, "isOldEnoughToDrinkAndDrive" returns whether a person of this given age is old enough to legally drink and drive in the United States. Notes:

- The legal drinking age in the United States is 21.
- It is always illegal to drink and drive in the United States.

```javascript
var output = isOldEnoughToDrinkAndDrive(22);
console.log(output); // --> false
```

```javascript
function isOldEnoughToDrinkAndDrive(age) {
      return false;
}
```

### Conditionals 2

#### checkAge

Write a function called "checkAge". Given a person's name and age, "checkAge" returns one of two messages: "Go home, {insert_name_here}!", if they are younger than 21. "Welcome, {insert_name_here}!", if they are 21 or older. Naturally, replace "{insert_name_here}" with the given name. :)

```javascript
var output = checkAge('Adrian', 22);
console.log(output); // --> 'Welcome, Adrian!'
```

```javascript
function checkAge(name, age) {
  if (age >= 21) {
  return 'Welcome, '+ name + '!';
  } else {
      return 'Go home, ' + name + '!';
  }
}
```

#### isGreaterThanTen

Write a function called "isGreaterThan10". Given a number, "isGreaterThan10" returns whether the given number is greater than 10.

```javascript
var output = isGreaterThan10(11);
console.log(output); // --> true
```

```javascript
function isGreaterThan10(num) {
  if (num > 10) {
      return true;
  } else {
      return false ;
  }
}
```

#### isLessThan30

Write a function called "isLessThan30". Given a number, "isLessThan30" returns whether the given number is less than 30.

```javascript
var output = isLessThan30(9);
console.log(output); // --> true
```

```javascript
function isLessThan30(num) {
  if (num < 30) {
      return true;
  } else {
      return false;
  }
}
```

#### equalsTen

Write a function called "equalsTen". Given a number, "equalsTen" returns whether or not the given number is 10.

```javascript
var output = equalsTen(9);
console.log(output); // --> false
```

```javascript
function equalsTen(num) {
  if (num === 10) {
      return true;
  } else {
      return false; 
  }
}
```
### Conditionals 3

#### isLessThan

Write a function called "isLessThan". Given 2 numbers, "isLessThan" returns whether num2 is less than num1.

```javascript
var output = isLessThan(9, 4);
console.log(output); // --> true
```

```javascript
function isLessThan(num1, num2) {
  if (num2 < num1) {
      return true;
  } else {
      return false;
  }
}
```

#### isGreaterThan

Write a function called "isGreaterThan". Given 2 numbers, "isGreaterThan" returns whether num2 is greater than num1.

```javascript
var output = isGreaterThan(11, 10);
console.log(output); // --> false
```

```javascript
function isGreaterThan(num1, num2) {
  if (num2 > num1) {
      return true;
  } else {
      return false;
  }
}
```

#### isEqualTo

Write a function called "isEqualTo". Given 2 numbers, "isEqualTo" returns whether num2 is equal to num1.

```javascript
var output = isEqualTo(11, 10);
console.log(output); // --> false
```

```javascript
function isEqualTo(num1, num2) {
  if (num2 === num1) {
      return true;
  } else {
      return false;
  }
}
```

#### isEven

Write a function called "isEven". Given a number, "isEven" returns whether it is even.

```javascript
var output = isEven(11);
console.log(output); // --> false
```

```javascript
function isEven(num) {
  if (num % 2 === 0) {
      return true;
  } else {
      return false;
  }
}
```

### Conditionals 4

#### isOdd

Write a function called "isOdd". Given a number, "isOdd" returns whether the given number is odd.

```javascript
var output = isOdd(9);
console.log(output); // --> true
```

```javascript
function isOdd(num) {
  if (num % 2 === 1) {
      return true;
  } else {
      return false;
  }
}
```

#### isSameLength

Write a function called "isSameLength".

Given two words, "isSameLength" returns whether the given words have the same length.

```javascript
var output = isSameLength('words', 'super');
console.log(output); // --> true
```

```javascript
function isSameLength(word1, word2) {
  if (word1.length === word2.length) {
      return true;
  } else {
      return false;
  }
}
```

#### areBothOdd

Write a function called "areBothOdd".

Given 2 numbers, "areBothOdd" returns whether or not both of the given numbers are odd.

```javascript
var output = areBothOdd(1, 3);
console.log(output); // --> true
```

```javascript
function areBothOdd(num1, num2) {
  // your code here
  if (num1 % 2 === 1 && num2 % 2 === 1) {
      return true;
  } else {
      return false;
  }
}
```

#### isEitherEven

Write a function called "isEitherEven".

Given two numbers, "isEitherEven" returns whether or not either one of the given numbers is even.

```javascript
var output = isEitherEven(1, 4);
console.log(output); // --> true
```

```javascript
function isEitherEven(num1, num2) {
  var num1IsEven = num1 % 2 === 0;
  var num2IsEven = num2 % 2 === 0;
  if (num1IsEven || num2IsEven) {
      return true;
  } else {
      return false;
  }
}
```

### Conditionals 5

#### isOddLength

Write a function called "isOddLength".

Given a word, "isOddLength" returns whether the length of the given word is odd.

```javascript
var output = isOddLength('special');
console.log(output); // --> true
```

```javascript
function isOddLength(word) {
  if (word.length % 2 === 1) {
      return true;
  } else {
      return false;
  }
}
```

#### isEvenLength
Submitted on 10/28/2021
Write a function called "isEvenLength".

Given a word, "isEvenLength" returns whether the length of the word is even.

```javascript
var output = isEvenLength('wow');
console.log(output); // --> false
```

```javascript
function isEvenLength(word) {
  if (word.length % 2 === 0) {
    return true;
  } else {
    return false;
  }
}
```

#### isEvenAndGreaterThan10

Write a function called "isEvenAndGreaterThanTen".

Given a number, "isEvenAndGreaterThanTen" returns whether it is both even and greater than 10.

```javascript
var output = isEvenAndGreaterThanTen(13);
console.log(output); // --> false
```

```javascript
function isEvenAndGreaterThanTen(num) {
  if (num % 2 === 0 && num > 10) {
    return true;
  } else {
    return false;
  }
}
```

### Conditionals 6

#### or

Write a function called "or".

Given 2 boolean expressions, "or" returns true or false, corresponding to the '||' operator. Notes:

- Do not use the || operator.
- Use ! and && operators instead.


```javascript
var output = or(true, false);
console.log(output); // --> true;
```


```javascript
function or(expression1, expression2) {
  return !(!expression1 && !expression2);
}
```

#### isEitherEvenOrAreBoth7

Write a function called "isEitherEvenOrAreBoth7".

Given two numbers, 'isEitherEvenOrAreBoth7' returns whether at least one of them is even, or, both of them are 7.

```javascript
var output = isEitherEvenOrAreBoth7(3, 7);
console.log(output); // --> false

var output = isEitherEvenOrAreBoth7(2, 3);
console.log(output); // --> true
```

```javascript
function isEitherEvenOrAreBoth7(num1, num2) {
  var atLeastOneEven = (num1 % 2 === 0) || (num2 % 2 ===0);
  var bothAre7 = (num1 ===7) && (num2 === 7);
  if (atLeastOneEven || bothAre7) {
    return true;
  } else {
    return false;
  }
}
```

#### isEitherEvenAndLessThan9

Write a function called "isEitherEvenAndLessThan9".

Given two numbers, 'isEitherEvenAndLessThan9' returns whether at least one of them is even, and, both of them are less than 9.

```javascript
var output = isEitherEvenAndLessThan9(2, 4);
console.log(output); // --> true

var output = isEitherEvenAndLessThan9(72, 2);
console.log(output); // --> false

```javascript
function isEitherEvenAndLessThan9(num1, num2) {
  var atLeastOneEven = (num1 % 2 === 0) || (num2 % 2 ===0);
  var bothLessThan9 = (num1 < 9) && (num2 < 9);
  if (atLeastOneEven && bothLessThan9) {
    return true;
  } else {
    return false;
  }
}
```

### Conditionals 7

#### areValidCredentials

Write a function called "areValidCredentials".

Given a name and a password, "areValidCredentials", returns true if the name is longer than 3 characters, AND, the password is at least 8 characters long. Otherwise it returns false.

```javascript
var output = areValidCredentials('Ritu', 'mylongpassword')
console.log(output); // --> true
```

```javascript
function areValidCredentials(name, password) {
  var nameValid = name.length > 3;
  var passwordValid = password.length >= 8;
  if (nameValid && passwordValid) {
    return true;
  } else {
    return false;
  }
}
```

#### findMinLengthOfThreeWords

Write a function called "findMinLengthOfThreeWords".

Given 3 words, "findMinLengthOfThreeWords" returns the length of the shortest word.

```javascript
var output = findMinLengthOfThreeWords('a', 'be', 'see');
console.log(output); // --> 1
```

```javascript
function findMinLengthOfThreeWords(word1, word2, word3) {
  var array = [word1, word2, word3];
  var minLength = word1.length;
  for (var i = 1 ; i < array.length; i++) {
      if (array[i].length < minLength) {
          minLength = array[i].length;
      }
  }
  return minLength;
}
```

#### findMaxLengthOfThreeWords

Write a function called "findMaxLengthOfThreeWords".

Given 3 words, "findMaxLengthOfThreeWords" returns the length of the longest word.

```javascript
var output = findMaxLengthOfThreeWords('a', 'be', 'see');
console.log(output); // --> 3
```

```javascript
function findMaxLengthOfThreeWords(word1, word2, word3) {
  var array = [word1, word2, word3];
  var maxLength = word1.length;
  for (var i = 1 ; i < array.length; i++) {
      if (array[i].length > maxLength) {
          maxLength = array[i].length;
      }
  }
  return maxLength;
}
```

### Conditionals 8

#### convertScoreToGrade

Write a function called "convertScoreToGrade".

Given a score, "convertScoreToGrade" returns a string representing the letter grade corresponding to the given score.

Notes:

(100 - 90) --> 'A'
(89 - 80) --> 'B'
(79 - 70) --> 'C'
(69 - 60) --> 'D'
(59 - 0) --> 'F'
If the given score is greater than 100 or less than 0, it should return 'INVALID SCORE'.

```javascript
ar output = convertScoreToGrade(91);
console.log(output); // --> 'A'
```

```javascript
function convertScoreToGrade(score) {
    if (score > 100 || score < 0) {
        return 'INVALID SCORE';
    }
    if (score <= 59) {
        return 'F';
    } else if (score <= 69) {
        return 'D';
    } else if (score <= 79) {
        return 'C';
    } else if (score <= 89) {
        return 'B';
    } else if (score <= 100) {
        return 'A';
    }
}
```

#### convertScoreToGradeWithPlus

Write a function called "convertScoreToGradeWithPlusAndMinus".

Given a score, "convertScoreToGradeWithPlusAndMinus" returns a string representing the letter grade corresponding to the given score.

Notes:

(100 - 90) --> 'A'
(89 - 80) --> 'B'
(79 - 70) --> 'C'
(69 - 60) --> 'D'
(59 - 0) --> 'F'
If the given score is greater than 100 or less than 0, it should return 'INVALID SCORE'.
If the score is between the 0 and 2 (inclusive) of a given range, return the letter with a '-'
If the score is between the 8 and 9 (inclusive) of a given range, return the letter with a '+'
There are is no F+ and there is no F-.

```javascript
var output = convertScoreToGradeWithPlusAndMinus(91);
console.log(output); // --> 'A-'
```

```javascript
function convertScoreToGradeWithPlusAndMinus(score) {
    if (score > 100 || score < 0) {
        return 'INVALID SCORE';
    }
    if (score <= 59) {
        return 'F';
    } else if (score <= 69) {
        if (score <= 62) {
            return 'D-';
        } else if (score >= 68) {
            return 'D+'
        } else {
            return 'D';
        } 
    } else if (score <= 79) {
        if (score <= 72) {
            return 'C-';
        } else if (score >= 78) {
            return 'C+';
        } else {
            return 'C';
        } 
    } else if (score <= 89) {
        if (score <= 82) {
            return 'B-';
        } else if (score >= 88) {
            return 'B+';
        } else {
            return 'B';
        } 
    } else if (score <= 100) {
        if (score <= 92) {
            return 'A-';
        } else if (score >= 98) {
            return 'A+';
        } else {
            return 'A';
        } 
    }
}
```

### Conditionals 9

#### getLongestOfThreeWords

Write a function called "getLongestOfThreeWords".

Given 3 words, "getLongestOfThreeWords" returns the longest of three words.

Notes:

- If there is a tie, it should return the first word in the tie.

```javascript
var output = getLongestOfThreeWords('these', 'three', 'words');
console.log(output); // --> 'these'
```

```javascript
function getLongestOfThreeWords(word1, word2, word3) {
  var words = [word1, word2, word3];
  var longest = words[0];
  for (var i = 1; i < words.length; i++) {
    if (words[i].length > longest.length) {
        longest = words[i];
    }
  }
  return longest;
}
```

#### findShortestOfThreeWords

Write a function called "findShortestOfThreeWords".

Given 3 strings, "findShortestOfThreeWords" returns the shortest of the given strings.

Notes:

- If there are ties, it should return the first word in the parameters list.

```javascript
var output = findShortestOfThreeWords('a', 'two', 'three');
console.log(output); // --> 'a'
```

```javascript
function findShortestOfThreeWords(word1, word2, word3) {
  if (word1.length <= word2.length) {
    if (word1.length <= word3.length) {
        return word1;
    } else {
        return word3;
    } 
  } else {
    if (word2.length <= word3.length) {
        return word2;
    } else {
        return words3
    }
  }
}
```

## Objects 1 - 13

### Objects 1

#### getProperty

Write a function called "getProperty". Given an object and a key, "getProperty" returns the value of the property at the given key. Notes:

- If there is no property at the given key, it should return undefined.

```javascript
var obj = {
  key: 'value'
};
var output = getProperty(obj, 'key');
console.log(output); // --> 'value'
```

```javascript
function getProperty(obj, key) {
  return obj[key];
}
```

#### addProperty

Write a function called "addProperty". Given an object, and a key, "addProperty" sets a new property on the given object with a value of true.

```javascript
var myObj = {};
addProperty(myObj, 'myProperty');
console.log(myObj.myProperty); // --> true
```

```javascript
function addProperty(obj, key) {
  return obj[key] = true;
}
```

#### removeProperty

Write a function called "removeProperty". Given an object and a key, "removeProperty" removes the given key from the given object.

```javascript
var obj = {
  name: 'Sam',
  age: 20
}
removeProperty(obj, 'name');
console.log(obj.name); // --> undefined
```

```javascript
function removeProperty(obj, key) {
  delete obj[key];
}
```

### Objects 2

#### addFullNameProperty

Write a function called "addFullNameProperty".

Given an object that has a "firstName" property and a "lastName" property, "addFullNameProperty" sets a "fullName" property on the input object, whose value is a string with the first name and last name separated by a space.

```javascript
var person = {
  firstName: 'Jade',
  lastName: 'Smith'
};
addFullNameProperty(person);
console.log(person.fullName); // --> 'Jade Smith'
```

```javascript
function addFullNameProperty(obj) {
  var firstName = obj.firstName;
  var lastName = obj.lastName;
  var fullName = firstName + ' ' + lastName;
  obj.fullName = fullName;
}
```

#### addObjectProperty

Write a function called "addObjectProperty".

Given two objects and a key, "addObjectProperty" sets a new property on the 1st object at the given key. The value of that new property is the entire 2nd object.

```javascript
var person1 = {
  name: 'Joe Blow',
  role: 'schlub'
};
var person2 = {
  name: 'Mr. Burns',
  role: 'supervisor'
};
addObjectProperty(person1, 'manager', person2);
console.log(person1.manager); // --> { name: 'Mr. Burns', role: 'supervisor' }
```

```javascript
function addObjectProperty(obj1, key, obj2) {
  obj1[key] = obj2;
}
```

#### isPersonOldEnoughToDrinkAndDrive

Write a function called "isPersonOldEnoughToDrinkAndDrive".

Given a "person" object, that contains an "age" property, "isPersonOldEnoughToDrinkAndDrive" returns whether the given person is old enough to legally drink and drive in the United States.

Notes:

- The legal drinking age in the United States is 21.
- The legal driving age in the United States is 16.
- It is ALWAYS illegal to drink and drive in the United States.

```javascript
var obj = {
  age: 45
};
var output = isPersonOldEnoughToDrinkAndDrive(obj);
console.log(output); // --> false
```

```javascript
function isPersonOldEnoughToDrinkAndDrive(person) {
  return false
}
```

### Objects 3

#### isPersonOldEnoughToDrive

Write a function called "isPersonOldEnoughToDrive".

Given a "person" object, that contains an "age" property, "isPersonOldEnoughToDrive" returns whether the given person is old enough to drive.

Notes:

- The legal driving age in the United States is 16.

```javascript
var obj = {
  age: 16
};
var output = isPersonOldEnoughToDrive(obj);
console.log(output); // --> true
```

```javascript
function isPersonOldEnoughToDrive(person) {
  if (person.age >= 16) {
      return true;
  } else {
      return false;
  }
}
```

#### isPersonOldEnoughToVote

Write a function called "isPersonOldEnoughToVote".

Given a "person" object, that contains an "age" property, "isPersonOldEnoughToVote" returns whether the given person is old enough to vote.

Notes:

- The legal voting age in the United States is 18.


```javascript
var obj = {
  age: 19
};
var output = isPersonOldEnoughToVote(obj);
console.log(output); // --> true
```

```javascript
function isPersonOldEnoughToVote(person) {
  // your code here
  if (person.age >= 18) {
      return true;
  } else {
      return false;
  }
}
```

#### addArrayProperty

Write a function called "addArrayProperty".

Given an object, a key, and an array, "addArrayProperty" sets a new property on the object at the given key, with its value set to the given array.

```javascript
var myObj = {};
var myArray = [1, 3];
addArrayProperty(myObj, 'myProperty', myArray);
console.log(myObj.myProperty); // --> [1, 3]
```

```javascript
function addArrayProperty(obj, key, arr) {
  obj[key] = arr;
}
```

### Objects 4

#### removeNumbersLargerThan

Write a function called "removeNumbersLargerThan".

Given a number and an object, "removeNumbersLargerThan" removes any properties whose values are numbers greater than the given number.


```javascript
var obj = {
  a: 8,
  b: 2,
  c: 'montana'
}
removeNumbersLargerThan(5, obj);
console.log(obj); // --> { b: 2, c: 'montana' }
```

```javascript
function removeNumbersLargerThan(num, obj) {
  for (var key in obj) {
    var value = obj[key];
    if (typeof value === "number" && value > num) {
        delete obj[key];
    }
  }
}
```

#### removeNumbersLessThan

Write a function called "removeNumbersLessThan".

Given a number and an object, "removeNumbersLessThan" removes any properties whose values are numbers less than the given number.

```javascript
var obj = {
  a: 8,
  b: 2,
  c: 'montana'
}
removeNumbersLessThan(5, obj);
console.log(obj); // --> { a: 8, c: 'montana' }
```

```javascript
function removeNumbersLessThan(num, obj) {
  for (var key in obj) {
    if (typeof obj[key] == "number" && obj[key] < num) {
        delete obj[key];
    }
  }
}
```

#### removeStringValuesLongerThan

Write a function called "removeStringValuesLongerThan".

Given an number and an object, "removeStringValuesLongerThan" removes any properties on the given object whose values are strings longer than the given number.

```javascript
var obj = {
  name: 'Montana',
  age: 20,
  location: 'Texas'
};
removeStringValuesLongerThan(6, obj);
console.log(obj); // { age: 20, location: 'Texas' }
```

```javascript
function removeStringValuesLongerThan(num, obj) {
  for (var key in obj) {
    if (typeof obj[key] == "string" && obj[key].length > num) {
      delete obj[key];
    }
  }
}
```

### Objects 5

#### removeEvenValues

Write a function called "removeEvenValues".

Given an object, "removeEvenValues" removes any properties whose values are even numbers.

Do this in place and return the original object, do not construct a cloned object that omits the properties.

Example:

```javascript
var obj = {
  a: 2,
  b: 3,
  c: 4
};
removeEvenValues(obj);
console.log(obj); // --> { b: 3 }
```

```javascript
function removeEvenValues(obj) {
  for (var key in obj) {
    if (typeof obj[key] == "number" && obj[key] % 2 == 0) {
        delete obj[key];
    }
  }
}
```

#### countNumberOfKeys

Write a function called "countNumberOfKeys".

Given an object, "countNumberOfKeys" returns how many properties the given object has.

```javascript
var obj = {
  a: 1,
  b: 2,
  c: 3
};
var output = countNumberOfKeys(obj);
console.log(output); // --> 3
```

```javascript
function countNumberOfKeys(obj) {
  var count = 0;
  for (var key in obj) {
      count += 1;
  }
  return count;
}
```

#### removeOddValues

Write a function called "removeOddValues".

Given an object, "removeOddValues" removes any properties whose values are odd numbers.

```javascript
var obj = {
  a: 2,
  b: 3,
  c: 4
};
removeOddValues(obj);
console.log(obj); // --> { a: 2, c: 4 }
```

```javascript
function removeOddValues(obj) {
  for (var key in obj) {
    if ( typeof obj[key] == "number" && obj[key] % 2 == 1) {
        delete obj[key];
    }
  }
}
```

### Objects 7

#### getElementsThatEqual10AtProperty

Write a function called "getElementsThatEqual10AtProperty".

Given an object and a key, "getElementsThatEqual10AtProperty" returns an array containing all the elements of the array located at the given key that are equal to ten.

Notes:

- If the array is empty, it should return an empty array.
- If the array contains no elements that are equal to 10, it should return an empty array.
- If the property at the given key is not an array, it should return an empty array.
- If there is no property at the key, it should return an empty array.

```javascript
var obj = {
  key: [1000, 10, 50, 10]
};
var output = getElementsThatEqual10AtProperty(obj, 'key');
console.log(output); // --> [10, 10]
```

```javascript
function getElementsThatEqual10AtProperty(obj, key) {
  if (obj[key] === undefined) {
    return [];
  }
  if (Array.isArray(obj[key]) === false) {
    return [];
  }
  if (obj[key].length === 0) {
    return [];
  }
  var result = [];
  for (var i = 0; i < obj[key].length; i++) {
    if (obj[key][i] === 10) {
        result.push(obj[key][i]);
    }
  }
  return result;
}
```

#### getElementsLessThan100AtProperty

Write a function called "getElementsLessThan100AtProperty".

Given an object and a key, "getElementsLessThan100AtProperty" returns an array containing all the elements of the array located at the given key that are less than 100.

Notes:

- If the array is empty, it should return an empty array.
- If the array contains no elements less than 100, it should return an empty array.
- If the property at the given key is not an array, it should return an empty array.
- If there is no property at the key, it should return an empty array.

```javascript
var obj = {
  key: [1000, 20, 50, 500]
};
var output = getElementsLessThan100AtProperty(obj, 'key');
console.log(output); // --> [20, 50]
```

```javascript
function getElementsLessThan100AtProperty(obj, key) {
  if (obj[key] === undefined) {
    return [];
  }
  if (Array.isArray(obj[key]) === false) {
    return [];
  }
  if (obj[key].length === 0) {
    return [];
  }
  var result = [];
  for (var i = 0; i<obj[key].length; i++) {
    if (obj[key][i] < 100) {
        result.push(obj[key][i]);
    }
  }
  return result;
}
```

### Objects 8

#### getElementsGreaterThan10AtProperty

Write a function called "getElementsGreaterThan10AtProperty".

Given an object and a key, "getElementsGreaterThan10AtProperty" returns an array containing the elements within the array, located at the given key, that are greater than 10.

Notes:

- If the array is empty, it should return an empty array.
- If the array contains no elements greater than 10, it should return an empty array.
- If the property at the given key is not an array, it should return an empty array.
- If there is no property at the key, it should return an empty array.

```javascript
var obj = {
  key: [1, 20, 30]
};
var output = getElementsGreaterThan10AtProperty(obj, 'key');
console.log(output); // --> [20, 30]
```

```javascript
function getElementsGreaterThan10AtProperty(obj, key) {
  if (obj[key] === undefined) {
    return [];
  }
  if (Array.isArray(obj[key]) === false) {
    return [];
  }
  if (obj[key].length === 0) {
    return [];
  }
  var result = [];
  for (var i = 0; i<obj[key].length; i++) {
    if (obj[key][i] > 10) {
        result.push(obj[key][i]);
    }
  }
  return result;
}
```

#### getFirstElementOfProperty

Write a function called "getFirstElementOfProperty".

Given an object and a key, "getFirstElementOfProperty" returns the first element of the array located at the given key.

Notes:

- If the array is empty, it should return undefined.
- If the property at the given key is not an array, it should return undefined.
- If there is no property at the key, it should return undefined.

```javascript
var obj = {
  key: [1, 2, 4]
};
var output = getFirstElementOfProperty(obj, 'key');
console.log(output); // --> 1
```

```javascript
function getFirstElementOfProperty(obj, key) {
  if (obj[key] === undefined) {
    return undefined;
  }
  if (Array.isArray(obj[key]) === false) {
    return undefined;
  }
  if (obj[key].length === 0) {
    return undefined;
  }
  return obj[key][0];
}
```

#### getNthElementOfProperty

Write a function called "getNthElementOfProperty".

Given an object and a key, "getNthElementOfProperty" returns the nth element of an array located at the given key.

Notes:

- If the array is empty, it should return undefined.
- If n is out of range, it should return undefined.
- If the property at the given key is not an array, it should return undefined.
- If there is no property at the key, it should return undefined.

```javascript
var obj = {
  key: [1, 2, 6]
};
var output = getNthElementOfProperty(obj, 'key', 1);
console.log(output); // --> 2
```

```javascript
function getNthElementOfProperty(obj, key, n) {
  if (obj[key] === undefined) {
    return undefined;
  }
  if (Array.isArray(obj[key]) === false) {
    return undefined;
  }
  return obj[key][n];
}
```

#### getLastElementOfProperty

Write a function called "getLastElementOfProperty".

Given an object and a key, "getLastElementOfProperty" returns the last element of an array located at the given key.

Notes:

If the array is empty, it should return undefined.
if the property at the given key is not an array, it should return undefined.
If there is no property at the key, it should return undefined.

```javascript
var obj = {
  key: [1, 2, 5]
};
var output = getLastElementOfProperty(obj, 'key');
console.log(output); // --> 5
```

```javascript
function getLastElementOfProperty(obj, key) {
  if (obj[key] === undefined) {
    return undefined;
  }
  if (Array.isArray(obj[key]) === false) {
    return undefined;
  }
  var lastElement = obj[key].length - 1;
  return obj[key][lastElement];
}
```

### Objects 9

#### getOddLengthWordsAtProperty

Write a function called "getOddLengthWordsAtProperty".

Given an object and a key, "getOddLengthWordsAtProperty" returns an array containing all the odd length word elements of the array located at the given key.

Notes:

- If the array is empty, it should return an empty array.
- If it contains no odd length elements, it should return an empty array.
- If the property at the given key is not an array, it should return an empty array.
- If there is no property at the given key, it should return an empty array.

```javascript
var obj = {
  key: ['It', 'has', 'some', 'words']
};
var output = getOddLengthWordsAtProperty(obj, 'key');
console.log(output); // --> ['has', 'words']
```

```javascript
function getOddLengthWordsAtProperty(obj, key) {
  if (obj[key] === undefined) {
    return [];
  }
  if (Array.isArray(obj[key]) === false) {
    return [];
  }
  var result = [];
  for (var i = 0; i<obj[key].length; i++) {
    if (obj[key][i].length % 2 === 1) {
        result.push(obj[key][i])
    }
  }
  return result;
}
```

#### getAverageOfElementsAtProperty

Write a function called "getAverageOfElementsAtProperty".

Given an object and a key, "getAverageOfElementsAtProperty" returns the average of all the elements in the array located at the given key.

Notes:

- If the array at the given key is empty, it should return 0.
- If the property at the given key is not an array, it should return 0.
- If there is no property at the given key, it should return 0.

```javascript
var obj = {
  key: [1, 2, 3]
};
var output = getAverageOfElementsAtProperty(obj, 'key');
console.log(output); // --> 2
```

```javascript
function getAverageOfElementsAtProperty(obj, key) {
  if (obj[key] === undefined) {
    return 0;
  }
  if (Array.isArray(obj[key]) === false) {
    return 0;
  }
  if (obj[key].length === 0) {
    return 0;
  }
  var sum = 0;
  for (var i = 0; i<obj[key].length; i++){
    sum += obj[key][i];
  }
  return sum/obj[key].length;
}
```

#### getEvenLengthWordsAtProperty

Write a function called "getEvenLengthWordsAtProperty".

Given an object and a key, "getEvenLengthWordsAtProperty" returns an array containing all the even length word elements of the array located at the given key.

Notes:

- If the array is empty, it should return an empty array.
- If it contains no even length elements, it should return an empty array.
- If the property at the given key is not an array, it should return an empty array.
- If there is no property at the key, it should return an empty array.

```javascript
var obj = {
  key: ['a', 'long', 'game']
};
var output = getEvenLengthWordsAtProperty(obj, 'key');
console.log(output); // --> ['long', 'game']
```

```javascript
function getEvenLengthWordsAtProperty(obj, key) {
  if (obj[key] === undefined) {
    return [];
  }
  if (Array.isArray(obj[key]) === false) {
    return [];
  }
  var result = [];
  for (var i = 0; i<obj[key].length; i++) {
    if (obj[key][i].length % 2 === 0) {
        result.push(obj[key][i])
    }
  }
  return result;
}
```

### Objects 10

#### getSquaredElementsAtProperty

Write a function called "getSquaredElementsAtProperty".

Given an object and a key, "getSquaredElementsAtProperty" returns an array containing all the squared elements of the array located at the given key.

Notes:

- If the array is empty, it should return an empty array.
- If the property at the given key is not an array, it should return an empty array.
- If there is no property at the key, it should return an empty array.

```javascript
var obj = {
  key: [2, 1, 5]
};
var output = getSquaredElementsAtProperty(obj, 'key');
console.log(output); // --> [4, 1, 25]
```

```javascript
function getSquaredElementsAtProperty(obj, key) {
  if (obj[key] === undefined) {
    return [];
  }
  if (Array.isArray(obj[key]) === false) {
    return [];
  }
  var result = [];
  var array = obj[key];
  for (var i = 0; i<array.length; i++) {
    var currentNum = array[i];
    var squaredNum = currentNum ** 2;
    result.push(squaredNum);
  }
  return result;
}
```

#### getOddElementsAtProperty

Write a function called "getOddElementsAtProperty".

Given an object and a key, "getOddElementsAtProperty" returns an array containing all the odd elements of the array located at the given key.

Notes:

- If the array is empty, it should return an empty array.
- If it contains no odd elements, it should return an empty array.
- If the property at the given key is not an array, it should return an empty array.
- If there is no property at the key, it should return an empty array.

```javascript
var obj = {
  key: [1, 2, 3, 4, 5]
};
var output = getOddElementsAtProperty(obj, 'key');
console.log(output); // --> [1, 3, 5]
```

```javascript
function getOddElementsAtProperty(obj, key) {
  if (obj[key] === undefined) {
    return [];
  }
  if (Array.isArray(obj[key]) === false) {
    return [];
  }
  var result = [];
  var array = obj[key];
  for (var i = 0; i<array.length; i++){
    if (obj[key][i] % 2 === 1) {
        result.push(obj[key][i]);
    }
  }
  return result;
}
```

#### getEvenElementsAtProperty
Submitted on 11/12/2021
Write a function called "getEvenElementsAtProperty".

Given an object and a key, "getEvenElementsAtProperty" returns an array containing all the even elements of the array located at the given key.

Notes:

- If the array is empty, it should return an empty array.
- If the array contains no even elements, it should return an empty array.
- If the property at the given key is not an array, it should return an empty array.
- If there is no property at the given key, it should return an empty array.

```javascript
var obj = {
  key: [1000, 11, 50, 17]
};
var output = getEvenElementsAtProperty(obj, 'key');
console.log(output); // --> [1000, 50]
```

```javascript
function getEvenElementsAtProperty(obj, key) {
  if (obj[key] === undefined) {
    return [];
  }
  if (Array.isArray(obj[key]) === false) {
    return [];
  }
  var result = [];
  var array = obj[key];
  for (var i = 0; i<array.length; i++) {
    if (obj[key][i] % 2 === 0) {
        result.push(obj[key][i]);
    }
  }
  return result;
}
```

### Objects 11

#### getSmallestElementAtProperty

Write a function called "getSmallestElementAtProperty".

Given an object and a key, "getSmallestElementAtProperty" returns the smallest element in the array located at the given key.

Notes:

- If the array is empty, it should return undefined.
- If the property at the given key is not an array, it should return undefined.
- If there is no property at the key, it should return undefined.

```javascript
var obj = {
  key: [2, 1, 5]
};
var output = getSmallestElementAtProperty(obj, 'key');
console.log(output); // --> 1

```javascript
function getSmallestElementAtProperty(obj, key) {
  if (obj[key] === undefined) {
    return undefined;
  }
  if (Array.isArray(obj[key]) === false) {
    return undefined;
  }
  if (obj[key].length === 0) {
    return undefined;
  }
  var smallestElement = obj[key][0];
  for (var i = 1; i < obj[key].length; i++){
    if (obj[key][i] < smallestElement) {
        smallestElement = obj[key][i];
    }
  }
  return smallestElement;
}
```

#### getLargestElementAtProperty

Write a function called "getLargestElementAtProperty".

Given an object and a key, "getLargestElementAtProperty" returns the largest element in the array located at the given key.

Notes:

- If the array is empty, it should return undefined.
- If the property at the given key is not an array, it should return undefined.
- If there is no property at the key, it should return undefined.

```javascript
var obj = {
  key: [1, 2, 4]
};
var output = getLargestElementAtProperty(obj, 'key');
console.log(output); // --> 4
```

```javascript
function getLargestElementAtProperty(obj, key) {
  if (obj[key] === undefined) {
    return undefined;
  }
  if (Array.isArray(obj[key]) === false) {
    return undefined;
  }
  if (obj[key].length === 0) {
    return undefined;
  }
  var largest = obj[key][0];
  for (var i = 1; i < obj[key].length; i++) {
    if (obj[key][i] > largest) {
        largest = obj[key][i];
    }
  }
  return largest;
}
```

#### getAllButLastElementOfProperty

Write a function called "getAllButLastElementOfProperty".

Given an object and a key, "getAllButLastElementOfProperty" returns an array containing all but the last element of the array located at the given key.

Notes:

- If the array is empty, it should return an empty array.
- If the property at the given key is not an array, it return an empty array.
- If there is no property at the key, it should return an empty array.

```javascript
var obj = {
  key: [1, 2, 3]
};
var output = getAllButLastElementOfProperty(obj, 'key');
console.log(output); // --> [1,2]
```

```javascript
function getAllButLastElementOfProperty(obj, key) {
  if (obj[key] === undefined) {
    return [];
  }
  if (Array.isArray(obj[key]) === false) {
    return [];
  }
  if (obj[key].length === 0) {
    return [];
  }
  obj[key].pop();
  return obj[key];
}
```

#### getElementOfArrayProperty

Write a function called "getElementOfArrayProperty".

Given an object, a key, and a numerical index, "getElementOfArrayProperty" returns the value of the element at the given index of the array located within the given object at the given key.

Notes:

- If the array is empty, it should return undefined.
- If the given index is out of range of the array located at the given key, it should return undefined.
- If the property at the given key is not an array, it should return undefined.
- If there is no property at the key, it should return undefined.

```javascript
var obj = {
 key: ['Jamil', 'Albrey']
};
var output = getElementOfArrayProperty(obj, 'key', 0);
console.log(output); // --> 'Jamil'
```

```javascript
function getElementOfArrayProperty(obj, key, index) {
  if (obj[key] === undefined) {
    return undefined;
  }
  if (Array.isArray(obj[key]) === false) {
    return undefined;
  }
  if (obj[key].length === 0) {
    return undefined;
  }
  return obj[key][index];
}
```

### Objects 12

#### getProductOfAllElementsAtProperty

Write a function called "getProductOfAllElementsAtProperty".

Given an object and a key, "getProductOfAllElementsAtProperty" returns the product of all the elements in the array located at the given key.

Notes:

- If the array is empty, it should return 0.
- If the property at the given key is not an array, it should return 0.
- If there is no property at the given key, it should return 0.

```javascript
var obj = {
  key: [1, 2, 3, 4]
};
var output = getProductOfAllElementsAtProperty(obj, 'key');
console.log(output); // --> 24
```

```javascript
function getProductOfAllElementsAtProperty(obj, key) {
  if (obj[key] === undefined) {
    return 0;
  }
  if (Array.isArray(obj[key]) === false) {
    return 0;
  }
  if (obj[key].length === 0) {
    return 0;
  }
  var product = 1;
  for (var i = 0; i<obj[key].length; i++){
    product *= obj[key][i];
  }
  return product;
}
```

### Objects 13

#### getSumOfAllElementsAtProperty

Write a function called "getSumOfAllElementsAtProperty".

Given an object and a key, "getSumOfAllElementsAtProperty" returns the sum of all the elements in the array located at the given key.

Notes:

- If the array is empty, it should return 0.
- If the property at the given key is not an array, it should return 0.
- If there is no property at the key, it should return 0.

```javascript
var obj = {
  key: [4, 1, 8]
};
var output = getSumOfAllElementsAtProperty(obj, 'key');
console.log(output); // --> 13
```

```javascript
function getSumOfAllElementsAtProperty(obj, key) {
  if (obj[key] === undefined) {
    return 0;
  }
  if (Array.isArray(obj[key]) === false) {
    return 0;
  }
  if (obj[key].length === 0) {
    return 0;
  }
  var sum = 0;
  for (var i = 0; i<obj[key].length; i++) {
    sum += obj[key][i];
  }
  return sum;
}
```

## String Methods 1 - 3

### String Methods 1

#### getFullName

Write a function called "getFullName". Given a first and a last name, "getFullName" returns a single string with the given first and last names separated by a single space.

```javascript
var output = getFullName('Joe', 'Smith');
console.log(output); // --> 'Joe Smith'
```

```javascript
function getFullName(firstName, lastName) {
  return firstName + " " + lastName;
}
```

#### getLengthOfWord

Write a function called "getLengthOfWord". Given a word, "getLengthOfWord" returns the length of the given word.

```javascript
var output = getLengthOfWord('some');
console.log(output); // --> 4
```

```javascript
function getLengthOfWord(word) {
  return word.length;
}
```

#### getLengthOfTwoWords

Write a function called "getLengthOfTwoWords". Given 2 words, "getLengthOfTwoWords" returns the sum of their lengths.

```javascript
var output = getLengthOfTwoWords('some', 'words');
console.log(output); // --> 9
```

```javascript
function getLengthOfTwoWords(word1, word2) {
  return word1.length + word2.length;
}
```

### String Methods 2

#### computeAverageLengthOfWords

Write a function called "computeAverageLengthOfWords".

Given two words, "computeAverageLengthOfWords" returns the average of their lengths.

```javascript
var output = computeAverageLengthOfWords('code', 'programs');
console.log(output); // --> 6
```

```javascript
function computeAverageLengthOfWords(word1, word2) {
  return (word1.length + word2.length ) / 2;
}
```

### String Methods 3

#### getLengthOfThreeWords

Write a function called "getLengthOfThreeWords".

Given 3 words, "getLengthOfThreeWords" returns the sum of their lengths.

```javascript
var output = getLengthOfThreeWords('some', 'other', 'words');
console.log(output); // --> 14
```

```javascript
function getLengthOfThreeWords(word1, word2, word3) {
  var sum = word1.length + word2.length + word3.length;
  return sum;
}
```

## Math 1 - 6

### Math 1

#### average

Write a function called "average".

Given two numbers, "average" returns their average.

```javascript
var output = average(4, 6);
console.log(output); // --> 5
average
Submitted on 10/28/2021
Write a function called "average".

Given two numbers, "average" returns their average.

var output = average(4, 6);
console.log(output); // --> 5
```

```javascript
function average(num1, num2) {
  return (num1 + num2) / 2;
}
```

#### computeAreaOfATriangle

Write a function called "computeAreaOfATriangle".

Given the base and height of a triangle, "computeAreaOfATriangle" returns its area.

```javascript
var output = computeAreaOfATriangle(4, 6);
console.log(output); // --> 12

```javascript
function computeAreaOfATriangle(base, height) {
  return (base * height) / 2;
}
```

#### cube

Write a function called "cube".

Given a number, "cube" returns the cube of that number.

```javascript
var output = cube(3);
console.log(output); // --> 27
```

```javascript
function cube(num) {
  return num ** 3;
}
```

#### square

Write a function called "square".

Given a number, "square" should return the square of the given number.

```javascript
var output = square(5);
console.log(output); // --> 25
```

```javascript
function square(num) {
  return num ** 2;
}
```

### Math 2

#### computeAreaOfARectangle

Write a function called "computeAreaOfARectangle".

Given the length and width of a rectangle, "computeAreaOfARectangle" returns its area.

```javascript
var output = computeAreaOfARectangle(4, 8);
console.log(output); // --> 32
```

```javascript
function computeAreaOfARectangle(length, width) {
  return length * width;
}
```

#### computePerimeterOfARectangle

Write a function called "computePerimeterOfARectangle".

Given a length and a width describing a rectangle, "computePerimeterOfARectangle" returns its perimeter.

```javascript
var output = computePerimeterOfARectangle(5, 2);
console.log(output); // --> 14
```

```javascript
function computePerimeterOfARectangle(length, width) {
  return (length + width) * 2;
}
```

#### computePerimeterOfATriangle

Write a function called "computePerimeterOfATriangle".

Given 3 sides describing a triangle, "computePerimeterOfATriangle" returns its perimeter.

```javascript
var output = computePerimeterOfATriangle(6, 7, 10);
console.log(output); // --> 23
```

```javascript
function computePerimeterOfATriangle(side1, side2, side3) {
  return side1 + side2 + side3;
}
```

### Math 3

#### computeTripledAreaOfARectangle

Write a function called "computeTripledAreaOfARectangle".

Given a length and width of a rectangle, "computeTripledAreaOfARectangle" returns the rectangle's area, multiplied by 3.

```javascript
var output = computeTripledAreaOfARectangle(2, 4);
console.log(output); // --> 24
```

```javascript
function computeTripledAreaOfARectangle(length, width) {
  return length * width * 3;
}
```

#### computePerimeterOfACircle

Write a function called "computePerimeterOfACircle".

Given the radius of a circle, "computePerimeterOfACircle" returns its perimeter.

Notes:

- Math.PI can be used for pi.

```javascript
var output = computePerimeterOfACircle(4);
console.log(output); // --> 25.132741228718345
```

Reference: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/PI

```javascript
function computePerimeterOfACircle(radius) {
  return 2 * Math.PI * radius;
}
```

#### computeAreaOfACircle

Write a function called "computeAreaOfACircle".

Given the radius of a circle, "computeAreaOfACircle" returns its area.

Notes:

Math.PI can be used for pi.

```javascript
var output = computeAreaOfACircle(4);
console.log(output); // --> 50.26548245743669
```

Reference: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/PI

```javascript
function computeAreaOfACircle(radius) {
  // your code here
  return Math.PI * (radius ** 2);
}
```

### Math 4

## Array Methods 1 - 16
## Array String Methods 1 - 2
## Advanced 1 - 8
## Interation 1 - 6
## Convert Array To Object 1 - 3
## Convert Object To Array 1 - 3

 
