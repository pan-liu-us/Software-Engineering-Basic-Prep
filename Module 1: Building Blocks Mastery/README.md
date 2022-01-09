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
/*
hints: De Morgan's laws
!(A && B) ---> !A || !B
!(A || B) ---> !A && !B
*/

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
### Objects 6

#### removeArrayValues

Write a function called "removeArrayValues".

Given an object, "removeArrayValues" removes any properties whose values are arrays.

```javascript
var obj = {
  a: [1, 3, 4],
  b: 2,
  c: ['hi', 'there']
}
removeArrayValues(obj);
console.log(obj); // --> { b: 2 }
```

```javascript
function removeArrayValues(obj) {
  for (var keys in obj) {
      if (Array.isArray(obj[keys])) {
          delete obj[keys];
      }
  }
}
```

#### removeNumberValues

Write a function called "removeNumberValues".

Given an object, "removeNumberValues" removes any properties whose values are numbers.

```javascript
var obj = {
  a: 2,
  b: 'remaining',
  c: 4
};
removeNumberValues(obj);
console.log(obj); // --> { b: 'remaining' }
```

```javascript
function removeNumberValues(obj) {
  for (var keys in obj) {
      if (typeof obj[keys] === "number") {
          delete obj[keys];
      }
  }  
}
```

#### removeStringValues

Write a function called "removeStringValues".

Given an object, "removeStringValues" removes any properties on the given object whose values are strings.

```javascript
var obj = {
  name: 'Sam',
  age: 20
}
removeStringValues(obj);
console.log(obj); // { age: 20 }
```

```javascript
function removeStringValues(obj) {
  for (var keys in obj) {
      if (typeof obj[keys] === "string") {
          delete obj[keys];
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

#### computePower

Write a function called "computePower".

Given a number and an exponent, "computePower" returns the given number, raised to the given exponent.

```javascript
var output = computePower(2, 3);
console.log(output); // --> 8
```

```javascript
function computePower(num, exponent) {
  return Math.pow(num, exponent);
}
```

#### computeSquareRoot

Write a function called "computeSquareRoot". Given a number, "computeSquareRoot" returns its square root.

```javascript
var output = computeSquareRoot(9);
console.log(output); // --> 3
```

```javascript
function computeSquareRoot(num) {
  return Math.sqrt(num);
}
```

#### doubleSquareRootOf

Write a function called "doubleSquareRootOf". Given a number, "doubleSquareRootOf" returns double its square root.

```javascript
var output = doubleSquareRootOf(121);
console.log(output); // --> 22
```

```javascript
function doubleSquareRootOf(num) {
  return Math.sqrt(num) * 2;
}
```

### Math 5

#### calculateBillTotal

Write a function called "calculateBillTotal".

Given the pre tax and pre tip amount of a meal, "calculateBillTotal" returns the total amount due after tax and tip.

Notes:

- Assume that sales tax is 9.5% and tip is 15%.
- Do NOT tip on the sales tax, only on the pre tip amount.

```javascript
var output = calculateBillTotal(20);
console.log(output); // --> 24.9
```

```javascript
function calculateBillTotal(preTaxAndTipAmount) {
  var salesTax = preTaxAndTipAmount * .095;
  var tip = preTaxAndTipAmount * .15;
  return preTaxAndTipAmount + salesTax + tip;
}
```

### Math 6

#### computeCompoundInterest

Write a function called "computeCompoundInterest".

Given a principal, an interest rate, a compounding frequency, and a time (in years), "computeCompoundInterest" returns the amount of compound interest generated.

```javascript
var output = computeCompoundInterest(1500, .043, 4, 6);
console.log(output); // --> 438.8368221341061
```

Reference: https://en.wikipedia.org/wiki/Compound_interest#Calculation_of_compound_interest This shows the formula used to calculate the total compound interest generated.

```javascript
function computeCompoundInterest(principal, interestRate, compoundingFrequency, timeInYears) {
  // P' - P = P * (1 + r/n) ^ nt - P
  var CompoundInterest = (principal * Math.pow((1 + (interestRate/compoundingFrequency)), (timeInYears * compoundingFrequency))) - principal;
  return CompoundInterest;
}
```

## Array Methods 1 - 16

### Array Methods 1

#### getNthElement

Write a function called "getNthElement".

Given an array and an integer, "getNthElement" returns the element at the given integer, within the given array.

Notes:

- If the array has a length of 0, it should return 'undefined'.

```javascript
var output = getNthElement([1, 3, 5], 1);
console.log(output); // --> 3
```

```javascript
function getNthElement(array, n) {
    eturn array[n];
}
```

#### getFirstElement

Write a function called "getFirstElement".

Given an array, "getFirstElement" returns the first element of the given array.

Notes:

- If the given array has a length of 0, it should return undefined.

```javascript
var output = getFirstElement([1, 2, 3, 4, 5]);
console.log(output); // --> 1
```

```javascript
function getFirstElement(array) {
    return array[0];
}
```

#### getLastElement

Write a function called "getLastElement".

Given an array, "getLastElement" returns the last element of the given array.

Notes:

- If the given array has a length of 0, it should return 'undefined'.

```javascript
var output = getLastElement([1, 2, 3, 4]);
console.log(output); // --> 4
```

```javascript
function getLastElement(array) {
  var index = array.length - 1;
  return array[index];
}
```

### Array Methods 2

#### addToFront

Write a function called "addToFront".

Given an array and an element, "addToFront" adds the given element to the front of the given array, and returns the given array.

Notes:

- It should be the SAME array, not a new array.
- In order to do this you should be familiar with the 'unshift' method.

```javascript
var output = addToFront([1, 2], 3);
console.log(output); // -> [3, 1, 2]
```

```javascript
function addToFront(arr, element) {
  arr.unshift(element);
  return arr;
}
```

#### addToBack

Write a function called "addToBack".

Given an array and an element, "addToBack" returns the given array with the given element added to the end.

Notes:

- It should be the SAME array, not a new array.
- In order to do this you should be familiar with the 'push' method.

```javascript
var output = addToBack([1, 2], 3);
console.log(output); // -> [1, 2, 3]
```

```javascript
function addToBack(arr, element) {
  arr.push(element);
  return arr;
}
```

### Array Methods 3

#### joinArrays

Write a function called "joinArrays".

Given two arrays, "joinArrays" returns an array with the elements of "arr1" in order, followed by the elements in "arr2".

```javascript
var output = joinArrays([1, 2], [3, 4]);
console.log(output); // --> [1, 2, 3, 4]
```

You should be familiar with the "concat" method for this problem.

```javascript
function joinArrays(arr1, arr2) {
  return arr1.concat(arr2);
}
```

#### getElementsAfter

Write a function called "getElementsAfter".

Given an array and an index, "getElementsAfter" returns a new array with all the elements after (but not including) the given index.

Notes:

- In order to do this you should be familiar with the 'slice' method.

```javascript
var output = getElementsAfter(['a', 'b', 'c', 'd', 'e'], 2);
console.log(output); // --> ['d', 'e']
```

```javascript
function getElementsAfter(array, n) {
  return array.slice( n + 1);
}
```

#### getElementsUpTo

Write a function called "getElementsUpTo".

Given an array and a index, "getElementsUpTo", returns an array with all the elements up until, but not including, the element at the given index.

Notes:

- In order to do this you should be familiar with the 'slice' method.

```javascript
var output = getElementsUpTo(['a', 'b', 'c', 'd', 'e'], 3)
console.log(output); // --> ['a', 'b', 'c']
```

```javascript
function getElementsUpTo(array, n) {
  return array.slice(0, n);
}
```

### Array Methods 4

#### getAllElementsButFirst

Write a function called "getAllElementsButFirst".

Given an array, "getAllElementsButFirst" returns an array with all the elements but the first.

```javascript
var input = [1, 2, 3, 4];
var output = getAllElementsButFirst(input);
console.log(output); // --> [2, 3, 4]
```

```javascript
function getAllElementsButFirst(array) {
  return array.slice(1);
}
```

#### getAllElementsButLast

Write a function called "getAllElementsButLast".

Given an array, "getAllElementsButLast" returns an array with all the elements but the last.

```javascript
var input = [1, 2, 3, 4];
var output = getAllElementsButLast(input);
console.log(output); // --> [1, 2 , 3]
```

```javascript
function getAllElementsButLast(array) {
  return array.slice(0, array.length - 1);
}
```

#### removeFromFront

Write a function called "removeFromFront".

Given an array, "removeFromFront" returns the given array with its first element removed.

Notes:

- You should be familiar with the method 'shift'.

```javascript
var output = removeFromFront([1, 2, 3]);
console.log(output); // --> [2, 3]
```

```javascript
function removeFromFront(arr) {
  arr.shift();
  return arr;
}
```

### Array Methods 5

#### removeFromBackOfNew

Write a function called "removeFromBackOfNew".

Given an array, "removeFromBackOfNew" returns a new array containing all but the last element of the given array.

Notes:

- You should be familiar with the 'slice' method.

```javascript
var arr = [1, 2, 3];
var output = removeFromBackOfNew(arr);
console.log(output); // --> [1, 2]
console.log(arr); // --> [1, 2, 3]
```

```javascript
function removeFromBackOfNew(arr) {
  var newArr = arr.slice();
  newArr.pop();
  return newArr;
}
```

#### removeFromFrontOfNew

Write a function called "removeFromFrontOfNew".

Given an array, "removeFromFrontOfNew" returns a new array containing all but the first element of the given array.

Notes:

- You should be familiar with the 'slice' method.

```javascript
var arr = [1, 2, 3];
var output = removeFromFrontOfNew(arr);
console.log(output); // --> [2, 3]
console.log(arr); // --> [1, 2, 3]
```

```javascript
function removeFromFrontOfNew(arr) {
  var newArr = arr.slice();
  newArr.shift();
  return newArr;
}
```

#### countCharacter

Write a function called "countCharacter".

Given a string input and a character, "countCharacter" returns the number of occurrences of a given character in the given string.

```javascript
var output = countCharacter('I am a hacker', 'a');
console.log(output); // --> 3
```

```javascript
function countCharacter(str, char) {
    var count = 0;
    for (var i = 0 ; i < str.length; i++) {
        if (str[i] === char) {
            count++;
        }
    }
    return count;
}
```

### Array Methods 6

#### removeFromBack

Write a function called "removeFromBack".

Given an array, "removeFromBack" returns the given array with its last element removed.

Notes:

- You should be familiar with the method 'pop'.

```javascript
var output = removeFromBack([1, 2, 3]);
console.log(output); // --> [1, 2]
```

```javascript
function removeFromBack(arr) {
  arr.pop()；
  return arr;
}
```

### Array Methods 7

#### joinThreeArrays

Write a function called "joinThreeArrays".

Given three arrays, "joinThreeArrays" returns an array with the elements of "arr1" in order followed by the elements in "arr2" in order followed by the elements of "arr3" in order.

```javascript
var output = joinThreeArrays([1, 2], [3, 4], [5, 6]);
console.log(output); // --> [1, 2, 3, 4, 5, 6]
```

You should be familiar with the "concat" method for this problem.

```javascript
function joinThreeArrays(arr1, arr2, arr3) {
  var concatted = arr1.concat(arr2, arr3);
  return concatted;
}
```

#### addToFrontOfNew

Write a function called "addToFrontOfNew".

Given an array and an element, "addToFrontOfNew" returns a new array containing all the elements of the given array, with the given element added to the front.

Important: It should be a NEW array instance, not the original array instance.

```javascript
var input = [1, 2];
var output = addToFrontOfNew(input, 3);
console.log(output); // --> [3, 1, 2];
console.log(input); // --> [1, 2]
```

```javascript
function addToFrontOfNew(arr, element) {
  var copyOfArr = arr.slice();
  copyOfArr.unshift(element);
  return copyOfArr;
}
```

#### addToBackOfNew

Write a function called "addToBackOfNew".

Given an array and an element, "addToBackOfNew" returns a clone of the given array, with the given element added to the end.

Important: It should be a NEW array instance, not the original array instance.

```javascript
var input = [1, 2];
var output = addToBackOfNew(input, 3);
console.log(input); // --> [1, 2]
console.log(output); // --> [1, 2, 3]
```

```javascript
function addToBackOfNew(arr, element) {
  var copyOfArr = arr.slice();
  copyOfArr.push(element);
  return copyOfArr;
}
```

#### getAllElementsButNth

Write a function called "getAllElementsButNth".

Given an array and an index, "getAllElementsButNth" returns an array with all the elements but the nth.

```javascript
var output = getAllElementsButNth(['a', 'b', 'c'], 1);
console.log(output); // --> ['a', 'c']
```

```javascript
function getAllElementsButNth(array, n) {
  array.splice(n, 1);
  return array;
}
```

### Array Methods 8

#### removeElement

Write a function called "removeElement".

Given an array of elements, and a "discarder" parameter, "removeElement" returns an array containing the items in the given array that do not match the "discarder" parameter.

Notes:

- If all the elements match, it should return an empty array.
- If an empty array is passed in, it should return an empty array.

```javascript
var output = removeElement([1, 2, 3, 2, 1], 2);
console.log(output); // --> [1, 3, 1]
```

```javascript
function removeElement(array, discarder) {
    for (var i = 0; i < array.length; i++) {
        if (array[i] === discarder) {
            array.splice(i, 1);
            i--;
        }
    }
    return array;
}
```

#### keep

Write a function called "keep".

Given an array and a keeper element, "keep" returns an array containing the items that match the given keeper element.

Notes:

- If no elements match, "keep" should return an empty array.

```javascript
var output = keep([1, 2, 3, 2, 1], 2)
console.log(output); --> [2, 2]
```

```javascript
function keep(array, keeper) {
    for (var i = 0; i < array.length; i++) {
        if (array[i] !== keeper) {
            array.splice(i, 1);
            i--;
        }
    }
    return array;
}
```

#### computeAverageOfNumbers

Write a function called "computeAverageOfNumbers".

Given an array of numbers, "computeAverageOfNumbers" returns their average.

Notes:

- If given an empty array, it should return 0.

```javascript
var input = [1,2,3,4,5];
var output = computeAverageOfNumbers(input);
console.log(output); // --> 3
```

```javascript
function computeAverageOfNumbers(nums) {
    if (nums.length === 0) {
        return 0;
    }
  
    var sum = 0;
    for (var i = 0; i<nums.length; i++) {
        sum += nums[i];
    }
    return sum / nums.length;
}
```

### Array Methods 9

#### filterOddLengthWords

Write a function called "filterOddLengthWords".

Given an array of strings, "filterOddLengthWords" returns an array containing only the elements of the given array whose lengths are odd numbers.

```javascript
var output = filterOddLengthWords(['there', 'it', 'is', 'now']);
console.log(output); // --> ['there', "now']
```

```javascript
function filterOddLengthWords(words) {
    var oddLengthWords = [];
    for (var i = 0; i < words.length; i++) {
        if (words[i].length % 2 === 1) {
            oddLengthWords.push(words[i]);
        } 
    }
    return oddLengthWords;
}
```

#### filterEvenLengthWords

Write a function called "filterEvenLengthWords".

Given an array of strings, "filterEvenLengthWords" returns an array containing only the elements of the given array whose length is an even number.

```javascript
var output = filterEvenLengthWords(['word', 'words', 'word', 'words']);
console.log(output); // --> ['word', 'word']
```

```javascript
function filterEvenLengthWords(words) {
    var evenLengthWords = [];
    for (var i = 0; i < words.length; i++) {
        if (words[i].length % 2 === 0) {
            evenLengthWords.push(words[i]);
        }
    }
    return evenLengthWords;
}
```

#### getLengthOfLongestElement

Write a function called "getLengthOfLongestElement".

Given an array, "getLengthOfLongestElement" returns the length of the longest string in the given array.

Notes:

- It should return 0 if the array is empty.

```javascript
var output = getLengthOfLongestElement(['one', 'two', 'three']);
console.log(output); // --> 5
```

```javascript
function getLengthOfLongestElement(arr) {
    if (arr.length === 0) {
        return 0;
    }
    var longestString = arr[0];
    for (var i = 1; i < arr.length; i++) {
        if (arr[i].length > longestString.length) {
            longestString = arr[i];
        }
    }
    return longestString.length;
}
```

### Array Methods 10

#### squareElements

Write a function called "squareElements". Given an array of numbers, "squareElements" should return a new array where each element is the square of the element of the given array.

```javascript
var output = squareElements([1, 2, 3]);
console.log(output); // --> [1, 4, 9]
```

```javascript
function squareElements(arr) {
    var squared = [];
    for (var i = 0; i < arr.length; i++) {
        squared.push(arr[i] ** 2);
    }
    return squared;
}
```

#### filterOddElements

Write a function called "filterOddElements".

Given an array of numbers, "filterOddElements" returns an array containing only the odd numbers of the given array.

```javascript
var output = filterOddElements([1, 2, 3, 4, 5]);
console.log(output); // --> [1, 3, 5]
```

```javascript
function filterOddElements(arr) {
    var oddElements = [];
    for (var i = 0; i < arr.length; i++) {
        if (arr[i] % 2 === 1) {
            oddElements.push(arr[i]);
        }
    }
    return oddElements;
}
```

#### computeProductOfAllElements

Write a function called "computeProductOfAllElements".

Given an array of numbers, "computeProductOfAllElements" returns the products of all the elements in the given array.

Notes:

- If given array is empty, it should return 0.

```javascript
var output = computeProductOfAllElements([2, 5, 6]);
console.log(output); // --> 60
```

```javascript
function computeProductOfAllElements(arr) {
    if (arr.length === 0) {
        return 0;
    }
    var product = 1;
    for (var i = 0; i < arr.length; i++) {
        product *= arr[i];
    }
    return product;
}
```

### Array Methods 11

#### filterEvenElements

Write a function called "filterEvenElements".

Given an array of numbers, "filterEvenElements" returns an array containing only the even numbers of the given array.

```javascript
var output = filterEvenElements([2, 3, 4, 5, 6]);
console.log(output); // --> [2, 4, 6]
```

```javascript
function filterEvenElements(arr) {
    var evenElements = [];
    for (var i = 0; i < arr.length; i++) {
        if (arr[i] % 2 === 0) {
            evenElements.push(arr[i]);
        }
    } 
    return evenElements;
}
```
            
#### getLengthOfShortestElement

Write a function called "getLengthOfShortestElement".

Given an array, "getLengthOfShortestElement" returns the length of the shortest string in the given array.

Notes:

- It should return 0 if the array is empty.

```javascript
var output = getLengthOfShortestElement(['one', 'two', 'three']);
console.log(output); // --> 3
···

```javascript
function getLengthOfShortestElement(arr) {
    if (arr.length === 0){
        return 0;
    }
    var shortest = arr[0];
    for (var i = 1; i < arr.length; i++) {
        if (arr[i].length < shortest.length) {
            shortest = arr[i];
        }
    }
    return shortest.length;
}
···

#### getLongestElement

Write a function called "getLongestElement".

Given an array, "getLongestElement" returns the longest string in the given array.

Notes:

- If there are ties, it returns the first element to appear.
- If the array is empty, it should return an empty string.

```javascript
var output = getLongestElement(['one', 'two', 'three']);
console.log(output); // --> 'three'
```

```javascript
function getLongestElement(arr) {
    if (arr.length === 0) {
        return "";
    }
    var longest = arr[0];
    for (var i = 1; i<arr.length; i++){
        if (arr[i].length > longest.length){
           longest = arr[i];
        }
    }
    return longest;
}
```

### Array Methods 12

#### findSmallestElement

Write a function called "findSmallestElement".

Given an array of numbers, "findSmallestElement" returns the smallest number within the given array.

Notes:

- If the given array is empty, it should return 0.

```javascript
var output = findSmallestElement([4, 1, 9, 10]);
console.log(output); // --> 1
```

```javascript
function findSmallestElement(arr) {
    if (arr.length === 0){
        return 0;
    }
    var smallest = arr[0];
    for (var i = 1; i<arr.length; i++){
        if (arr[i] < smallest) {
            smallest = arr[i];
        }
    }
    return smallest;
}
```

#### findShortestElement

Write a function called "findShortestElement".

Given an array, "findShortestElement" returns the shortest string within the given array.

Notes:

- If there are ties, it should return the first element to appear.
- If the given array is empty, it should return an empty string.


var output = findShortestElement(['a', 'two', 'three']);
console.log(output); // --> 'a'

```javascript
function findShortestElement(arr) {
    if (arr.length === 0) {
        return "";
    }
    var shortest = arr[0];
    for (var i = 1; i<arr.length; i++) {
        if (arr[i].length < shortest.length) {
            shortest = arr[i];
        }
    }
    return shortest;
}
```

### Array Methods 13

#### getLargestElement

Write a function called "getLargestElement".

Given an array, "getLargestElement" returns the largest number in the given array.

Notes:

- It should return 0 if the array is empty.

```javascript
var output = getLargestElement([5, 2, 8, 3]);
console.log(output); // --> 8;
····

```javascript
function getLargestElement(arr) {
    if (arr.length === 0) {
        return 0;
    }
    var largest = arr[0];
    for (var i = 1; i<arr.length; i++) {
        if (arr[i] > largest) {
            largest = arr[i];
        }
    }
    return largest;
}
```

#### computeSumOfAllElements

Write a function called "computeSumOfAllElements".

Given an array of numbers, "computeSumOfAllElements" returns the sum of all the elements in the given array.

```javascript
var output = computeSumOfAllElements([1, 2, 3])
console.log(output); // --> 6
```

```javascript
function computeSumOfAllElements(arr) {
    var sum = 0;
    for (var i = 0; i<arr.length; i++){
        sum += arr[i];
    }
    return sum;
}
```

### Array Methods 14

#### joinArraysOfArrays
Submitted on 11/12/2021
Write a function called "joinArrayOfArrays".

Given an array of arrays, "joinArrayOfArrays" returns a single array containing the elements of the nested arrays.

```javascript
var output = joinArrayOfArrays([[1, 4], [true, false], ['x', 'y']]);
console.log(output); // --> [1, 4, true, false, 'x', 'y']
```

You should be familiar with the "concat" method for this problem.

```javascript
function joinArrayOfArrays(arr) {
    var result = [];
    for(var i = 0;i <arr.length; i++){
        result = result.concat(arr[i]);
    }
    return result;
}
```

### Array Methods 15

#### findShortestWordAmongMixedElements

Write a function called "findShortestWordAmongMixedElements".

Given an array, "findShortestWordAmongMixedElements" returns the shortest string within the given array.

Notes:

- If there are ties, it should return the first element to appear in the given array.
- Expect the given array to have values other than strings.
- If the given array is empty, it should return an empty string.
- If the given array contains no strings, it should return an empty string.

```javascript
var output = findShortestWordAmongMixedElements([4, 'two', 2, 'three']);
console.log(output); // --> 'two'
```

```javascript
function findShortestWordAmongMixedElements(arr) {
    if (arr.length === 0) {
        return "";
    }
    var strings = [];
    for (var i = 0; i<arr.length; i++) {
        if (typeof arr[i] === "string") {
            strings.push(arr[i]);
        }
    }
    if (strings.length === 0) {
        return "";
    }
  
    var shortest = strings[0];
  
    for (var i = 1; i<strings.length; i++) {
        if (strings[i].length < shortest.length) {
            shortest = strings[i];
        }
    }
    return shortest;
}
```

#### findSmallestNumberAmongMixedElements

Write a function called "findSmallestNumberAmongMixedElements".

Given an array of mixed elements, "findSmallestNumberAmongMixedElements" returns the smallest number within the given array.

Notes:

- If the given array is empty, it should return 0.
- If the array contains no numbers, it should return 0.


var output = findSmallestNumberAmongMixedElements([4, 'lincoln', 9, 'octopus']);
console.log(output); // --> 4

```javascript
function findSmallestNumberAmongMixedElements(arr) {
    if (arr.length === 0) {
        return 0;
    }
    var nums = [];
    for (var i = 0; i < arr.length; i++) {
        if (typeof arr[i] === "number") {
            nums.push(arr[i]);
        }
    }
    if (nums.length === 0) {
        return 0;
    }
    var smallest = nums[0];
    for (var i = 1; i<nums.length; i++) {
        if (nums[i] < smallest) {
            smallest = nums[i];
        }
    } 
    return smallest;
}
```

### Array Methods 16

#### getLongestWordOfMixedElements

Write a function called "getLongestWordOfMixedElements".

Given an array of mixed types, "getLongestWordOfMixedElements" returns the longest string in the given array.

Notes:

- If the array is empty, it should return an empty string ("").
- If the array contains no strings; it should return an empty string.

```javascript
var output = getLongestWordOfMixedElements([3, 'word', 5, 'up', 3, 1]);
console.log(output); // --> 'word'
```

```javascript
function getLongestWordOfMixedElements(arr) {
    if (arr.length === 0) {
        return "";
    }
    var words = [];
    for (var i = 0; i < arr.length; i++) {
       if (typeof arr[i] === "string") {
           words.push(arr[i]);
       }
   }
    if (words.length === 0) {
       return "";
    }
    var longest = words[0];
    for (var j = 0; j < words.length; j++) {
        if (words[j].length > longest.length) {
            longest = words[j];
        }
    }
    return longest;
}
```

#### getLargestNumberAmongMixedElements

Write a function called "getLargestNumberAmongMixedElements".

Given any array, "getLargestNumberAmongMixedElements" returns the largest number in the given array.

Notes:

- The array might contain values of a type other than numbers.
- If the array is empty, it should return 0.
- If the array contains no numbers, it should return 0.

```javascript
var output = getLargestNumberAmongMixedElements([3, 'word', 5, 'up', 3, 1]);
console.log(output); // --> 5
```

```javascript
function getLargestNumberAmongMixedElements(arr) {
    if (arr.length === 0) {
        return 0;
    }
    var nums = [];
    for (var i = 0; i < arr.length; i++) {
        if (typeof arr[i] === "number") {
            nums.push(arr[i]);
        }
    }
    if (nums.length === 0) {
        return 0;
    }
    var largest = nums[0];
    for (var j = 0; j < nums.length; j++) {
        if (nums[j] > largest) {
            largest = nums[j];
        }
    }
    return largest;
}
```

## Array String Methods 1 - 2

### Array String Methods 1

#### getAllLetters

Write a function called "getAllLetters".

Given a word, "getAllLetters" returns an array containing every character in the word.

Notes:

If given an empty string, it should return an empty array.
You should be familiar with the 'split' method.

```javascript
var output = getAllLetters('Radagast');
console.log(output); // --> ['R', 'a', 'd', 'a', 'g', 'a', 's', 't']
```

```javascript
function getAllLetters(str) {
    if (str === "") {
        return str = [];
    }
    var splitted = str.split("");
    return splitted;
}
```

#### getAllWords

Write a function called "getAllWords".

Given a sentence, "getAllWords" returns an array containing every word in the sentence.

Notes:

- If given an empty string, it should return an empty array.
- You should be familiar with the 'split' method.

```javascript
var output = getAllWords('Radagast the Brown');
console.log(output); // --> ['Radagast', 'the', 'Brown']
```

```javascript
function getAllWords(str) {
    if (str === "") {
        return str = [];
    }
    var splitted = str.split(" ");
    return splitted;
}
```

### Array String Methods 2

#### convertDoubleSpaceToSingle

Write a function called "convertDoubleSpaceToSingle".

Given a string, "convertDoubleSpaceToSingle" returns the passed in string, with all the double spaces converted to single spaces.

```javascript
var output = convertDoubleSpaceToSingle("string  with  double  spaces");
console.log(output); // --> "string with double spaces"
```

Notes:

- In order to do this problem, you should be familiar with "String.split", and "Array.join".

```javascript
function convertDoubleSpaceToSingle(str) {
    var split = str.split("  ");
    var joined = split.join(" ");
    return joined;
}
```

## Advanced 1 - 8

### Advanced 1

#### countWords

Write a function called "countWords".

Given a string, "countWords" returns an object where each key is a word in the given string, with its value being how many times that word appeared in the given string.

Notes:

- If given an empty string, it should return an empty object.

```javascript
var output = countWords('ask a bunch get a bunch');
console.log(output); // --> {ask: 1, a: 2, bunch: 2, get: 1}
```

```javascript
function countWords(str) {
    if (str === "") {
        return {};
    }
    var result = {};
    var words = str.split(" ");
    for (var i = 0 ; i < words.length ; i++) {
        if (result[words[i]] === undefined) {
            result[words[i]] = 1;
        } else { 
            result[words[i]] += 1;
        }
    }
    return result;
}
```

### Advanced 2

#### extend

Write a function called "extend".

Given two objects, "extend" adds properties from the 2nd object to the 1st object.

Notes:

- Add any keys that are not in the 1st object.
- If the 1st object already has a given key, ignore it (do not overwrite the property value).
- Do not modify the 2nd object at all.

```javascript
var obj1 = {
  a: 1,
  b: 2
};
var obj2 = {
  b: 4,
  c: 3
};

extend(obj1, obj2);

console.log(obj1); // --> {a: 1, b: 2, c: 3}
console.log(obj2); // --> {b: 4, c: 3}
```

```javascript
function extend(obj1, obj2) {
    for (var keyFromObj2 in obj2) {
        if (obj1[keyFromObj2] === undefined) {
            obj1[keyFromObj2] = obj2[keyFromObj2];
        }  
    }
}
```

### Advanced 3

#### select

Write a function called "select".

Given an array and an object, "select" returns a new object whose properties are those in the given object AND whose keys are present in the given array.

Notes:

- If keys are present in the given array, but are not in the given object, it should ignore them.
- It does not modify the passed in object.

```javascript
var arr = ['a', 'c', 'e'];
var obj = {
  a: 1,
  b: 2,
  c: 3,
  d: 4
};
var output = select(arr, obj);
console.log(output); // --> { a: 1, c: 3 }
```

```javascript
function select(arr, obj) {
    var result = {};
    for (var i = 0; i<arr.length; i++) {
        if (obj[arr[i]] !== undefined) {
            result[arr[i]] = obj[arr[i]];
        }
    }
    return result;
}
```

### Advanced 4

#### countAllCharacters

Write a function called "countAllCharacters".

Given a string, "countAllCharacters" returns an object where each key is a character in the given string. The value of each key should be how many times each character appeared in the given string.

Notes:

- If given an empty string, countAllCharacters should return an empty object.

```javascript
var output = countAllCharacters('banana');
console.log(output); // --> {b: 1, a: 3, n: 2}
```

```javascript
function countAllCharacters(str) {
    var result = {};
    for (var i = 0; i < str.length; i++) {
        if (result[str[i]] === undefined) {
            result[str[i]] = 1;
        } else {
            result[str[i]] += 1;
        }
    }
    return result;
}
```

### Advanced 5

#### sumDigits

Write a function called "sumDigits".

Given a number, "sumDigits" returns the sum of all its digits.

```javascript
var output = sumDigits(1148);
console.log(output); // --> 14
```

If the number is negative, the first digit should count as negative.

```javascript
var output = sumDigits(-316);
console.log(output); // --> 4
```

Notes:

- In order to use some of the methods that will be most helpful to you, you will most likely want to do some string to number conversion and vice versa.
- Be sure to familiarize yourself with the "toString" method, as well as the "Number" function.

```javascript
function sumDigits(num) {
    var inputIsNegative = false;
    if (num < 0) {
        num = Math.abs(num);
        inputIsNegative = true;
    }
    var total = 0;
    var numString = num.toString();
    var firstValue = Number(numString[0]);
    for(var i=0; i < numString.length; i++) {
        total += Number(numString[i]);
    }
    if (inputIsNegative) {
        total = total - (2 * firstValue);
        return total;
    } else {
        return total;
    }
}
```

### Advanced 6

#### modulo

Write a function called "modulo".

Given 2 numbers, "modulo" returns the remainder after dividing num1 by num2.

It should behave as described in the canonical documentation (MDN) for the JavaScript remainder operator: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Remainder_()

Notes:

- Do NOT use the actual built-in modulo (aka "remainder") operator (%) in your implementation.
- 0 % ANYNUMBER = 0.
- ANYNUMBER % 0 = NaN.
- If either operand is NaN, then the result is NaN.
- Modulo always returns the sign of the first number, even if the remainder is 0.

```javascript
var output = modulo(25, 4);
console.log(output); // --> 1
```

```javascript
function modulo(num1, num2) {
    if (num1 === 0) {
        return 0;
    }
    if (num2 === 0) {
        return NaN;
    }
    if (isNaN(num2) || isNaN(num1)) {
        return NaN;
    }
    // create a resultIsPositive boolean flog
    var resultIsPositive = true;
    if (num1 < 0) {
        resultIsPositive = false;  
    }
    // make both num1 and num2 positive versions
    num1 = Math.abs(num1);
    num2 = Math.abs(num2);
    // reassign num1 ri be num1 - num2, until num1 < num2
    while (num1 >= num2) {
        num1 = num1 - num2;
    }
    // check if result is positive
    if (resultIsPositive) {
        return num1;
    } else {
        return -num1;
    }
}
```

### Advanced 7

#### isOddWithoutModulo

Write a function called "isOddWithoutModulo".

Given a number, "isOddWithoutModulo" returns whether the passed in number is odd.

Note:

- It does so without using the modulo operator (%).
- It should work for negative numbers and zero.

```javascript
var output = isOddWithoutModulo(17);
console.log(output); // --> true
```

```javascript
function isOddWithoutModulo(num) {
    if (num === 0) {
        return false;
    }
    num = Math.abs(num);
    while (num >= 2) {
        num = num - 2;
    }
    if (num === 1) {
        return true;
    } else {
        return false;
    }
}
```

### Advanced 8

#### isEvenWithoutModulo

Write a function called "isEvenWithoutModulo".

Given a number, "isEvenWithoutModulo" returns whether it is even.

Notes:

- It does so without using the modulo operator (%).
- It should work for negative numbers and zero.

```javascript
var output = isEvenWithoutModulo(8);
console.log(output); // --> true
```

```javascript
function isEvenWithoutModulo(num) {
    if (num === 0) {
        return true;
    }
    num = Math.abs(num);
    while (num >= 2) {
        num -= 2;
    }
    if (num === 0) {
        return true;
    } else {
        return false;
    }
}
```

## Interation 1 - 6

### Interation 1

#### getIndexOf

Write a function called "getIndexOf".

Given a character and a string, "getIndexOf" returns the first position of the given character in the given string.

Notes:

- Strings are zero indexed, meaning the first character in a string is at position 0.
- When a string contains more than one occurrence of a character, it should return the index of its first occurrence.
- If the character does not exist in the string, it should return -1.
- Do not use the native indexOf function in your implementation.

```javascript
var output = getIndexOf('a', 'I am a hacker');
console.log(output); // --> 2
```

```javascript
function getIndexOf(char, str) {
    for ( var i = 0; i < str.length; i++){
        if (str[i] === char) {
            return i;
        }
    }
    return -1;
}
```

### Iteration 2

#### getStringLength

Write a function called "getStringLength".

Given a string, "getStringLength" returns the length of the given string.

Notes:

- Do NOT use any native 'length' methods.
- You might consider using 'substring' or 'slice' as alternatives.

```javascript
var output = getStringLength('hello');
console.log(output); // --> 5
```


### Iteration 3

#### computeSummationToN

Write a function called "computeSummationToN".

Given a number, "computeSummationToN" returns the sum of sequential numbers leading up to the given number, beginning at 0.

Notes:

- If n = 4, it should calculate the sum of 1 + 2 + 3 + 4, and return 10.

```javascript
var output = computeSummationToN(6);
console.log(output); // --> 21
```

```javascript
function computeSummationToN(n) {
   var sum = 0;
   for (var i = 1; i <= n; i++) {
        sum += i;
    }
    return sum;
}
```

### Iteration 4

#### computeFactorialOfN

Write a function called "computeFactorialOfN".

Given a natural number (a whole number greater than 0), "computeFactorialOfN" returns its factorial.

```javascript
var output = computeFactorialOfN(3);
console.log(output); // --> 6

var output = computeFactorialOfN(4);
console.log(output); // --> 24
```

```javascript
function computeFactorialOfN(n) {
    var factorial = 1;
    for (i = 1; i <= n; i++) {
        factorial *= i;
    }
    return factorial;
}
```

#### repeatString

Write a function called "repeatString".

Given a string and a number, "repeatString" returns the given string repeated the given number of times.

```javascript
var output = repeatString('code', 3);
console.log(output); // --> 'codecodecode'
```

```javascript
function repeatString(string, num) {
    // repeat num times of string
    var result = "";
    for (i = 1 ; i <= num; i++) {
    result += string;
    }
    return result;
}
```

### Iteration 5

#### multiply

Write a function called "multiply".

Given 2 numbers, "multiply" returns their product.

Notes:

- It should not use the multiply operator - *

```javascript
var output = multiply(4, 7);
console.log(output); // --> 28
```

```javascript
function multiply(num1, num2) {
    var resultIsPositive = true;
    if ((num1 > 0 && num2 < 0) || (num1 < 0 && num2 > 0)) {
        resultIsPositive = false;
    }
    num1 = Math.abs(num1);
    num2 = Math.abs(num2);
    var result = 0;
    for (var i = 1; i <= num2; i++) {
        result += num1;
    }
    if (resultIsPositive) {
        return result;
    } else {
        return -result;
    }
}
```

### Iteration 6

#### multiplyBetween

Write a function called "multiplyBetween".

Given 2 integers, "multiplyBetween" returns the product between the two given integers, beginning at num1, and excluding num2.

Notes:

- The product between 1 and 4 is 1 * 2 * 3 = 6.
- If num2 is not greater than num1, it should return 0.

```javascript
var output = multiplyBetween(2, 5);
console.log(output); // --> 24
```

```javascript
function multiplyBetween(num1, num2) {
    if (num2 <= num1) {
        return 0;
    }
    var product = 1;
    for (var i = num1; i < num2; i++) {
       product *= i;
    }
    return product;
}
```

#### computeSumBetween

Write a function called "computeSumBetween".

Given 2 integers, "computeSumBetween" returns the sum between the two given integers, beginning at num1, and excluding num2.

Notes:

- The sum between 1 and 4 is 1 + 2 + 3 = 6.
- If num2 is not greater than num1, it should return 0.

```javascript
var output = computeSumBetween(2, 5);
console.log(output); // --> 9
```

```javascript
function computeSumBetween(num1, num2) {
    if (num2 <= num1) {
        return 0;
    }
    var sum = 0;
    for (var i = num1; i < num2; i++) {
       sum += i;
    }
    return sum;
}
```

## Convert Array To Object 1 - 3

#### Convert Array To Object 1

Write a function 'transformFirstAndLast' that takes in an array, and returns an object with:

1. the first element of the array as the object's key, and
2. the last element of the array as that key's value.
Example input:

```javascript
var input = ['Queen', 'Elizabeth', 'Of Hearts', 'Beyonce'];
```

Function's return value (output):

```javascript
{
  Queen : 'Beyonce'
}
```

Do not change the input array. Assume all elements in the input array will be of type 'string'.

Note that the input array may have a varying number of elements. Your code should flexibly accommodate that.

E.g. it should handle input like:

```javascript
['Kevin', 'Bacon', 'Love', 'Hart', 'Costner', 'Coleman']
```

Function's return value (output):

```javascript
{
  Kevin : 'Coleman'
}
```

```javascript
function transformFirstAndLast(array) {
    var transformed = {};
    // result[key] = value
    transformed[array[0]] = array[array.length - 1];
    return transformed;
}
```
#### Convert Array To Object 2

Convert Array To Object 2
Submitted on 12/01/2021
Write a function 'transformArrayToObject' which takes in an array of arrays, and returns an object with each pair of elements in the array as a key-value pair.

Example input:

```javascript
var input = [['make', 'Ford'], ['model', 'Mustang'], ['year', 1964]];
```

Function's return value (output):

```javascript
{
  make : 'Ford',
  model : 'Mustang',
  year : 1964
}
```

Do not change the input string. Assume that all elements in the array will be of type 'string'.

Note that the input may have a different number of elements than the given sample. For instance, if the input had 6 values instead of 4, your code should flexibly accommodate that.

```javascript
function transformArrayToObject(array) {
    var transformed = {};
    for (i = 0; i < array.length; i++) {
        transformed[array[i][0]] = array[i][1];
    }
    return transformed;
}
```

#### Convert Array To Object 3

Write a function called "transformEmployeeData" that transforms some employee data from one format to another.

The argument will look like this:

```javascript
var input = [
    [
        ['firstName', 'Joe'], ['lastName', 'Blow'], ['age', 42], ['role', 'clerk']
    ],
    [
        ['firstName', 'Mary'], ['lastName', 'Jenkins'], ['age', 36], ['role', 'manager']
    ]
];
```

Given that input, the return value should look like this:

```javascript
[
    {firstName: 'Joe', lastName: 'Blow', age: 42, role: 'clerk'},
    {firstName: 'Mary', lastName: 'Jenkins', age: 36, role: 'manager'}
]
```

Note that the input may have a different number of rows or different keys than the given sample.

For example, let's say the HR department adds a "tshirtSize" field to each employee record. Your code should flexibly accommodate that.

```javascript
function transformEmployeeData(employeeData) {
    var employeeArray = [];
    for (var i = 0; i < employeeData.length; i++) {
        personArray = employeeData[i];
        var personObj = {};
        for (var j = 0; j < personArray.length; j++) {
            personObj[personArray[j][0]] = personArray[j][1];
        }
        employeeArray.push(personObj);
    }
    return employeeArray;
}
```

## Convert Object To Array 1 - 3

#### Convert Object To Array 1

Write a function called "getAllKeys" which returns an array of all the input object's keys. Example input:

```javascript
var input = {
  name : 'Sam',
  age : 25,
  hasPets : true
};
```

Function's return value (output) :

```javascript
['name', 'age', 'hasPets']
```

Do not use "Object.keys" to solve this prompt.

Note that your function should be able to handle any object passed in it.

E.g. it should also handle an input like:

```javascript
var alternativeInput = {
  a : 'a',
  number : 11,
  hungry : true,
  grammyWins : 1
};
```

Function's return value (output):

```javascript
['a', 'number', 'hungry', 'grammyWins']
```

```javascript
function getAllKeys(obj) {
    var keys = [];
    for (var key in obj) {
        keys.push(key);
    }
    return keys ;
}
```

#### Convert Object To Array 2

Write a function called "listAllValues" which returns an array of all the input object's values. Example input:

```javascript
var input = {
  name : 'Krysten',
  age : 33,
  hasPets : false
};
```

Function's return value (output):

```javascript
['Krysten', 33, false]
```

Do not use "Object.values" to solve this prompt.

Note that the input may have a different number of keys and values than the given sample. E.g. it should also handle an input like:

```javascript
var alternativeInput = {
  a : 'a',
  number : 11,
  hungry : true,
  grammyWins : 1
};
```

Function's return value (output):

```javascript
['a', 11, true, 1]
```

```javascript
function listAllValues(obj) {
    var values = [];
    for (var key in obj) {
        values.push(obj[key]);
    }
    return values;
}
```

#### Convert Object To Array 3

Write a function called "convertObjectToArray" which converts an object literal into an array of arrays, like this:

Argument:

```javascript
var input = {
  name: 'Holly',
  age: 35,
  role: 'producer'
};
```

Return value:

```javascript
[['name', 'Holly'], ['age', 35], ['role', 'producer']]
```

```javascript
function convertObjectToArray(obj) {
    var result = [];
    for (var key in obj) {
        var innerArray = [key,obj[key]];
        result.push(innerArray);
    }
    return result;
}
```

#### Greet Customer

Write a function called "greetCustomer".

Given a name, "greetCustomer" returns a greeting based on how many times that customer has visited the restaurant. Please refer to the customerData object.

The greeting should be different, depending on the name on their reservation.

Case 1 - Unknown customer ( Name is not present in customerData ):

```javascript
var output = greetCustomer('Terrance');
console.log(output); // --> 'Welcome! Is this your first time?'
```

Case 2 - Customer who has visited only once ( 'visits' value is 1 ):

```javascript
var output = greetCustomer('Joe');
console.log(output); // --> 'Welcome back, Joe! We're glad you liked us the first time!'
```

Case 3 - Repeat customer: ( 'visits' value is greater than 1 ):

```javascript
var output = greetCustomer('Carol');
console.log(output); // --> 'Welcome back, Carol! So glad to see you again!'

Notes:

- Your function should not alter the customerData object to update the number of visits.
- Do not hardcode to the exact sample data. This is a BAD IDEA:

```javascript
if (firstName === 'Joe') {
  // do something
}
```

```javascript
var customerData = {
  'Joe': {
    visits: 1
  },
  'Carol': {
    visits: 2
  },
  'Howard': {
    visits: 3,
  },
  'Carrie': {
    visits: 4
  }
};

function greetCustomer(firstName) {
  if (customerData[firstName] === undefined) {
      return 'Welcome! Is this your first time?';
  }
  if (customerData[firstName].visits === 1) {
      return `Welcome back, ${firstName}! We're glad you liked us the first time!`;
  } else {
      return `Welcome back, ${firstName}! So glad to see you again!`;
  }
}
```


