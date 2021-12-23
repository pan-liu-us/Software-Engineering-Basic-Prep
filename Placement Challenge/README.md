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

Complete the function `indexOfArray`. This function will take in two parameters, an array and an element, and returns the index, inside of the array, where the element is located. You will want to use the `indexOf` method for Arrays. If the element is not present within array, your function should return -1.

```javascript
function indexOfArray(array, item) {
  return array.indexOf(item);
}
```

#### Join an Array into a String | Using join

Complete a function that takes in two parameters, an array and a string. Your function should call join on the input array with an argument of the input string, and return the results.

```javascript
function useJoin(array, string) {
  return array.join(string);
}
```

#### Add a Property to an Object

Complete a function that takes in three parameters, an object, and a string (which will represent a key), and a value. Your function should add a property to the inputted object. The key of this property should be the inputted string parameter, and the value of this property should be the inputted value. Your function should then return the inputted object.

```javascript
function addProperty(obj, key, value) {
  obj[key] = value;
  return obj;
}
```

#### Remove a Property from an Object

omplete a function that takes in two parameters, an object, and a string (which will represent a key). Your function should remove (delete) the property located at the inputted key. Your function should then return the inputted object.

```javascript
function removeProperty(obj, key) {
  delete obj[key];
  return obj;
}
```

#### Iterate over an Object

Complete a function that takes in one parameter, an object. Your function should iterate over the object, and log the values to the console. Your function need not return anything.

NOTE: DO NOT USE Object.keys, or Object.values in your solution.

```javascript
function iterateOverObject(obj) {
  for (key in obj) {
      console.log(obj[key]);
  }
}


/*
If we want to return an array of those values, we can do:

function iterateOverObject(obj) {  
  var array = [];
  for (key in obj) {
      array.push(obj[key]);
  }
  return array;
}

If we can use Object.values:

function iterateOverObject(obj) {
  return Object.values(obj);
}

*/
```

## Intermediate

#### Use an Object to count things

Complete a function called countAllCharacters. Given a string, your function returns an object where each key is a character in the given string. The value of each key should be how many times each character appeared in the given string.

Notes:

- If given an empty string, countAllCharacters should return an empty object.

```javascript
var output = countAllCharacters('banana');
console.log(output); // --> {b: 1, a: 3, n: 2}
```

```javascript
function countAllCharacters(str) {
  if (str.length === 0) {
      return {};
  } else {
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
}
```

More simple solution:

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

#### Convert a Complex Array to an Object

Write a function called transformEmployeeData that transforms some employee data from one format to another.

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
var result = [
    {firstName: 'Joe', lastName: 'Blow', age: 42, role: 'clerk'},
    {firstName: 'Mary', lastName: 'Jenkins', age: 36, role: 'manager'}
]
```

Note that the input may have a different number of rows (more employees) or different keys than the given sample.

```javascript
function transformEmployeeData(employeeData) {
  var result = [];
  for (var i = 0; i < employeeData.length; i++) {
      var employeeArr = employeeData[i];
      var employeeObj = {};
      for (var j = 0; j < employeeArr.length; j++) {
          employeeObj[employeeArr[j][0]] = employeeArr[j][1];
      }
      result.push(employeeObj);
  }
  return result;
}
```

#### Convert an Object to a Complex Array

Complete a function called convertObjectToArray which converts an object literal into an array of arrays, like this:

Argument:

```javascript
var input = {
  name: 'Holly',
  age: 35,
  role: 'producer'
}
```
Return value:

```javascript
var output = [['name', 'Holly'], ['age', 35], ['role', 'producer']]
```

Note that the input may have a different number of properties than the given sample.

```javascript
function convertObjectToArray(obj) {
  var result = [];
  for (var keys in obj) {
      var innerArray = [keys, obj[keys]];
      result.push(innerArray);
  }
  return result;
}
```

#### Cumulative Challenge

Complete a function called greetCustomers.

Given a name, greetCustomers returns a greeting based on how many times that customer has visited the restaurant. Please refer to the customerData object.

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
```

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

#### A Request From Corporate

Let us walk through the idea for this problem, as it is somewhat more complex than the first sections of this placement challenge. The problem will require you to write two functions. One function will accomplish a task of some kind, and the other function will be an assertion function which can be used to compare your answer with an expected answer.

The first function you will write will be called `generateSampleView`. The input for this function will always be an array of objects, theoretically the result of a call to an API, or database. `generateSampleView` will take this array as its parameter, and return an array of strings based upon conditions that we will describe in a moment. The format of this input array of objects is described below:

```javascript
var users = [
  {
    "id": 1,
    "name": "Leanne Graham",
    "username": "Bret",
    "email": "Sincere@april.biz",
    "address": {
      "street": "Kulas Light",
      "suite": "Apt. 556",
      "city": "Gwenborough",
      "zipcode": "92998-3874",
      "geo": {
        "lat": "-37.3159",
        "lng": "81.1496"
      }
    },
    "phone": "1-770-736-8031 x56442",
    "website": "hildegard.org",
    "company": {
      "name": "Romaguera-Crona",
      "catchPhrase": "Multi-layered client-server neural-net",
      "bs": "harness real-time e-markets"
    }
  },
  {
    "id": 2,
    "name": "Ervin Howell",
    "username": "Antonette",
    "email": "Shanna@melissa.tv",
    "address": {
      "street": "Victor Plains",
      "suite": "Suite 879",
      "city": "Wisokyburgh",
      "zipcode": "90566-7771",
      "geo": {
        "lat": "-43.9509",
        "lng": "-34.4618"
      }
    },
    "phone": "010-692-6593 x09125",
    "website": "anastasia.net",
    "company": {
      "name": "Deckow-Crist",
      "catchPhrase": "Proactive didactic contingency",
      "bs": "synergize scalable supply-chains"
    }
  }
];


// generateSampleView
function generateSampleView(sampleUsers) {
    let output = [];
    for (let j = 0; j < sampleUsers.length; j++) {
        if (sampleUsers[j]["id"] % 2 === 1) {
            output.push(sampleUsers[j]["email"])
        } else {
            output.push(getAddress(sampleUsers[j]["address"]))
        }
    }
    return output;
}

function getAddress(addressObj) {
    let address = "";
    address += addressObj["street"] + ", " + addressObj["suite"] + ", " + addressObj["city"] + ", " + addressObj["zipcode"];
    return address;
}


// assertArraysEqual
function assertArraysEqual(actual, expected, testName) {
    let sameLength = actual.length === expected.length;
    let sameValue = true;
    for (let i = 0; i < expected.length; i++) {
        if (actual[i] !== expected[i]) {
            sameValue = false;
            break;
        }
    }
    
    if (sameLength && sameValue) {
        console.log(`passed.`)
    } else {
        console.log(`failed [${testName}]. Expected ${expected}, but got ${actual}`)
    }
}

var actual_1 = generateSampleView(users);
var expected_1 = ["Sincere@april.biz", "Victor Plains, Suite 879, Wisokyburgh, 90566-7771"];
assertArraysEqual(actual_1,expected_1,"should display correct sample view.");
```

