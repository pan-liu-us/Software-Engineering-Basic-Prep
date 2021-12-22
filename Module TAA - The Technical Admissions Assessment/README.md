## Advanced Pre-Assessment Practice

#### Altitude Deltas

Please write a function that takes an array of integer altitudes along a hiking trail, as well as two indexes into that array. The two indexes represent the start and end of a segment in the array. We can assume that the array will only contain integers, and that the two indexes will be valid (i.e. they will exist in the input array, and will make sense compared to each other - start is before end).

Your function should return the "sum of the changes for a walk within that segment" (i.e., beginning at the start index and ending at the end index). Each integer in the array represents another height on the trail, so "walking" will mean accumulating each change in height into a "sum of the changes".

Note that increases in height count double.

Here are some examples of your code running, assuming you have successfully created the described function. Please be sure to name the function "sumAltitudeDeltas".

```javascript
let output_0 = sumAltitudeDeltas([1, 2, 3, 1], 0, 3);
console.log(output_0); //--> 6

let output_1 = sumAltitudeDeltas([5, 3, 6, 7, 2], 2, 4);
console.log(output_1); //--> 7

let output_2 = sumAltitudeDeltas([5, 3, 6, 7, 2], 0, 1);
console.log(output_2); //--> 2

let output_3 = sumAltitudeDeltas([5, 3, 6, 7, 2], 0, 4);
console.log(output_3); //--> 15

let output_4 = sumAltitudeDeltas([4, 1, 4, 0, 20, 13], 1, 4);
console.log(output_4); //--> 50
```

```javascript
function sumAltitudeDeltas(height, start, end) {
    let sum = 0;
    for (let i = start; i < end; i++) {
        let diff = height [i+1] - height[i];
        if (diff > 0) {
            sum += (diff * 2);
        } else {
            sum -= diff;
        }
    }
    return sum;
}
```

#### Check Winner for Connect Four

Write a function called 'checkWinner'. This function will take an array with a length of 7. Each element of the array will be either; 'red', 'black', or 0. We can assume that no violation of either of these is possible (i.e. input will always be of length 7, and elements will only be 'red', 'black', or 0).

Your function should accept this array as its only parameter.

If there are 4 'red' elements consecutively in a row, 'checkWinner' should return the string: 'Red Wins!'. Similarly, if there are 4 'black' elements consecutively in a row, 'checkWinner' should return the string: 'Black Wins!'. If neither of these is the case, 'checkWinner' should return 'Draw!'.

Here are some examples of your code running, assuming you have successfully created the described function. Please be sure to name the function "checkWinner".

```javascript
let blackWinner = checkWinner(['black', 'red', 'black', 'black', 'black', 'black', 'red']);
console.log(blackWinner); //-> 'Black Wins!'

let redWinner = checkWinner([0,0,0, 'red', 'red', 'red', 'red']);
console.log(redWinner); //-> 'Red Wins!'

let draw = checkWinner(['red', 'red', 'red', 'black', 'red', 'black', 0]);
console.log(draw); // -> 'Draw!'
```

```javascript
function checkWinner(array) {
    for (let i = 0; i < array.length; i++) {
        if (array[i] === "black" && array[i + 1] === "black" && array[i + 2] === "black" && array[i + 3] === "black") {
            return "Black Wins!";
        } else if (array[i] === "red" && array[i + 1] === "red" && array[i + 2] === "red" && array[i + 3] === "red") {
            return "Red Wins!";
        }
    }
    return "Draw!"
}
```

#### A Request From Corporate

Let us walk through the idea for this problem, as it is somewhat more complex than usual. The problem will require you to write two functions. One function will accomplish a task of some kind, and the other function will be an assertion function which can be used to compare your answer with an expected answer.

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
```

Note: your function will be tested with a longer input, but the format will remain consistent for each user in the input array.

Your function should examine each user object, and add to the array return value for this function one of the following:

- If the value of the id property is odd, add the user's email to the return array
- If the value of the id property is even, your function should create a new string for the given user, add the street, suite, city, and zipcode, each separated by a space and a comma, as one string, to the return array

Thus, if our input was the users array listed above, our output would be:

```javascript
var output = ["Sincere@april.biz", "Victor Plains, Suite 879, Wisokyburgh, 90566-7771"];
```

The second function you will write will be called `assertArraysEqual`. It will be a function that takes three parameters: `actual` will be an array of scalar values, and should ideally be the result of calling a function that you are testing. (presumably the function being tested should return an array of scalar values); `expected`, also an array of scalar values, should be the theoretical result of calling your function (or, what you "expect" the function to return). Finally, `testName` will be a string, and should describe what a call to `assertArraysEqual` is verifying about the function being tested.

Please DO NOT USE JSON.stringify(), Array.join(), or any other "convert both arrays to strings so I can compare two strings" type of technique to implement this.

There are typically two things that we must check in order to determine that two arrays of scalar values are indeed equal to one another. Do they have the same length, and do they contain the same values. Thus, your function must make a determination about these issues, then either log 'passed' to the console or else 'failed', as well as the testName to the console. The tests for this function will check to see if your console.log message for a passing case contains 'passed', and 'failed' for a failing case (both in lower case).

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

#### Comma Separated Integers

You are going to create a function called "solution", which will take in an array of increasing integers, and return them in the format described below.

A format for expressing an ordered list of integers is to use a comma separated list of either individual integers or a range of integers denoted by the starting integer separated from the end integer in the range by a dash, '-'.

The range includes all integers in the interval including both endpoints. It is not considered a range unless it spans at least 3 numbers.

For example, an input of `[12, 13, 15, 16, 17]` would return `"12, 13, 15-17"`

Complete the solution so that it takes a list of integers in increasing order and returns a correctly formatted string in the range format. Below is an example of your code running, assuming you have solved the problem correctly.

```javascript
solution([-6, -3, -2, -1, 0, 1, 3, 4, 5, 7, 8, 9, 10, 11, 14, 15, 17, 18, 19, 20]);
// returns "-6,-3-1,3-5,7-11,14,15,17-20"

solution([-4, -3, -2, -1, 2, 3, 5, 6, 12, 13, 14, 15, 17]);
// returns "-4--1,2,3,5,6,12-15,17"
```

```javascript
function solution(int) {
  if (int.length > 0 && int.length < 3) {
    return int.join(",");
  }

  let result = [];
  let start = 0;
  let next = 1;
  let end = 2;
  while (start < int.length) {
    if (int[end] - int[next] === 1 && int[next] - int[start] === 1) {
      while (int[end] - int[next] === 1) {
        next = end;
        end = end + 1;
      }
      let seq = int.slice(start,end);
      result.push(`${seq[0]}-${seq[seq.length-1]}`);
      start = end;
      next = end + 1;
      end = end + 2;
    } else {
      result.push(int[start]);
      start = next;
      next = end;
      end = end + 1;
    }
  }

  return result.join(",");

}

function assertEqual(actual, expected, testName) {
  if (actual === expected) {
    console.log(`passed`);
  } else {
    console.log(`FAILED [${testName}] Expected "${expected}",but got "${actual}"`)
  }
}

var actual_1 = solution([-6, -3, -2, -1, 0, 1, 3, 4, 5, 7, 8, 9, 10, 11, 14, 15, 17, 18, 19, 20]);
var expected_1 = "-6,-3-1,3-5,7-11,14,15,17-20";
assertEqual(actual_1, expected_1, 'should return formatted integers');

var actual_2 = solution([-4, -3, -2, -1, 2, 3, 5, 6, 12, 13, 14, 15, 17]);
var expected_2 = "-4--1,2,3,5,6,12-15,17"
assertEqual(actual_2, expected_2, 'should return formatted integers');
```

#### Split Strings

Complete the function `splitPairs` such that it splits the input string into pairs of characters. If the input string has a length that is odd, then it should replace the missing second character of the final pair with an underscore `_.` Note, an empty string should make your function produce an empty array.

```javascript
function splitPairs(input) {
  let inputArray = input.split('');
  let result = [];
  
  if(input.length === 0)
    return result;
    
  if (inputArray.length % 2 !== 0) {
    for (let i = 0; i < inputArray.length - 1; i += 2) {
      let pair = inputArray[i] + inputArray[i + 1];
      result.push(pair);
    }
    result.push(inputArray[inputArray.length - 1] + '_');    
  } else {
    for (let i = 0; i < inputArray.length; i += 2) {
      let pair = inputArray[i] + inputArray[i + 1];
      result.push(pair);
    }
  }
  
  return result;
}

console.log(splitPairs("")); // returns []

console.log(splitPairs("abcd")); // returns [ 'ab', 'cd' ]

console.log(splitPairs("abcde")); // returns [ 'ab', 'cd', 'e_' ]
```

Highest Scoring Word

Given a string of words, you need to find the highest scoring word.

Each letter of a word scores points according to its position in the alphabet: a = 1, b = 2, c = 3 etc.

You need to return the highest scoring word as a string.

If two words score the same, return the word that appears earliest in the original string.

All letters will be lowercase and all inputs will be valid.

```javascript
function highestScoringWord(string) {
    var words = string.split(' '),
	highestScore = 0,
	result = '';
	for (var i = 0; i < words.length; i++) {
	    var highestScoringWord  = words[i];
	    var score = 0;
	    for (var j = 0; j < highestScoringWord.length; j++)  {
	        score += (highestScoringWord.charCodeAt(j) - 96);
	    }
	    if (score > highestScore) {
	        highestScore = score;
	        result = highestScoringWord;
	    }
	  }
	 return result;
}

console.log(highestScoringWord("ab bc ac")); // returns bc
```

#### Extract a Domain Name

Write a function that when given a URL as a string, parses out just the domain name and returns it as a string. For example:

Input1: "http://github.com/carbonfive/raygun  " Output1: "github"

Input2: "http://www.zombie-bites.com  " Output2: "zombie-bites"

Input3: "https://www.cnet.com  " Output3: "cnet"

```javascript
function getDomain(url) {
  url = url.replace("https://", '');
  url = url.replace("http://", '');
  url = url.replace("www.", '');
  return url.split('.')[0];
};

function assertEqual(actual, expected, testName) {
  if (actual === expected) {
    console.log(`passed`);
  } else {
    console.log(`failed [${testName}], expected ${expected}, but got ${actual}`);
  }
}

url_1 = getDomain("http://github.com/carbonfive/raygun");
expected_1 = "github";
assertEqual(url_1,expected_1,"should return domain name");

url_2 = getDomain("http://www.zombie-bites.com");
expected_2 = "zombie-bites";
assertEqual(url_2,expected_2,"should return domain name");

url_3 = getDomain("https://www.cnet.com");
expected_3 = "cnet";
assertEqual(url_3,expected_3,"should return domain name")
```
