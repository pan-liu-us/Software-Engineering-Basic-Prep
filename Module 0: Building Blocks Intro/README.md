## Variables

#### Undefined

We will start with a walkthrough that should get you started with completing challenges in this Module, as well as beyond. The task is for you to write a function that returns `undefined`, but that task is already complete. 

```javascript
function nothing() {
  // returns undefined by default (NO ADDITIONAL CODE REQUIRED)
}
```

#### Booleans

Now we are going to complete a function that takes no parameters and returns true. 

```javascript
function returnTrue() {
  return true;
}
```

#### Numbers

Next, we are going to complete a function that takes one number parameter, adds two to that number, then returns the result.

```javascript
function addTwo(num) {
  return num + 2;
}
```

#### Strings

Lastly, we are going to complete a function that takes two parameters, a string and number (will refer to an index within the string). The function should return the character within the string, located at the given number index.

```javascript
function returnACharacter(string, index) {
  // returns string character at given index
  return string[index];
}
```

## Objects

### Arrays

#### Arrays 1

We are going to complete a function that takes in an array parameter, and returns it.

```javascript
function returnArray(array) {
  return array
}
```

#### Arrays 2

We are going to complete a function that takes in an array and a number (will refer to an index within the array). The function should return the element located within the array at the given number index.

```javascript
function returnAnElement(array, index) {
  // returns array element at given index
  return array[index];
}
```

#### Arrays 3

We are going to complete a function that takes no parameters. This function should create an array, and return it.

```javascript
function createAndReturnAnArray() {
  var size = ["S" , "M", "L"];
  return size;
}
```

### Objects

#### Objects 1

We are going to complete a function that takes in an object parameter, and returns it.

```javascript
function returnObject(object) {
  return object;
}
```

#### Objects 2

We are going to complete a function that takes in an object and a string (will refer to a key in the object). The function should return the value of the property located within the object at the given string key.

```javascript
function returnAValue(obj, key) {
  return obj[key];
}
```

#### Objects 3

We are going to complete a function that takes no parameters. This function should create an object, and return it.

```javascript
function createAndReturnAnObject() {
  // create an object
  // return the created object
  var birthday = {year: "2019", month: "01", day:"19"};
  return birthday;
}
```

#### Objects 4

We are going to write a function that returns the type of argument the function has been called with (assume the argument will be scalar - not a collection).

```javascript
function getType(param) {
  // returns the type of param
  return  typeof param;
}
```

#### Objects 5

We are going to write a function that returns true if the argument is an Array, and false if it is not

```javascript
function determineIsAnArray(input) {
  // assign result variable to call to Array.isArray
  // return result variable
  var result = Array.isArray(input);
  return result;
}
```

## Operators and Methods

### Working with Booleans

#### Using the 'not' operator

We are going to complete a function that takes in a boolean parameter, and returns the opposite. Below are examples of the code running, assuming that you will have completed the described function: `opposite`.

```javascript
var outputTrue = opposite(false);
console.log('should be true:', outputTrue);

var outputFalse = opposite(true);
console.log('should be false:', outputFalse);
```

```javascript
function opposite(boolean) {
  // returns the opposite of the inputted boolean value
  return !boolean;
}
```

#### Using the 'or' operator

We are going to complete a function that takes in two boolean parameters. Your function should create a variable and assign it to the result of comparing the two input parameters using the `||` operator, then return that variable. Below are examples of the code running, assuming that you will have completed the described function: `eitherAreTrue`.

```javascript
var outputTrue = eitherAreTrue(true, false);
console.log('should be true:', outputTrue);

var outputFalse = eitherAreTrue(false, false);
console.log('should be false:', outputFalse);
```

```javascript
function eitherAreTrue(bool_1, bool_2) {
  // create a result variable
  // assign it to bool_1 OR bool_2
  // return the result variable
  var result = bool_1 || bool_2;
  return result;
}
```

#### Using the 'and' operator

We are going to complete a function that takes in two boolean parameters. Your function should create a variable and assign it to the result of comparing the two input parameters using the `&&` operator, then return that variable. Below are examples of the code running, assuming that you will have completed the described function: `bothAreTrue`.

```javascript
var outputTrue = bothAreTrue(true, true);
console.log('should be true:', outputTrue);

var outputFalse = bothAreTrue(false, true);
console.log('should be false:', outputFalse);
```

```javascript
function bothAreTrue(bool_1, bool_2) {
  // create a result variable
  // assign it to bool_1 AND bool_2
  // return the result variable
  var result = bool_1 && bool_2;
  return result;
}
```

#### A Combination of Booleans

We are going to complete a function that takes in three boolean parameters (bool_1, bool_2, and bool_3). Your function should create a variable and assign it to the result of the following: bool_1 AND either bool_2 OR bool_3. Below are examples of the code running, assuming that you will have completed the described function: `combination`.

```javascript
var outputTrue = combination(true, true, false);
console.log('should be true:', outputTrue);

var outputFalse = combination(false, true, true);
console.log('should be false:', outputFalse);
```

```javascript
function combination(bool_1, bool_2, bool_3) {
  // create a result variable
  // assign it to bool_1 AND either bool_2 OR bool_3
  // return the result variable
  var result = bool_1 && (bool_2 || bool_3);
  return result;
}
```

#### Equal to | Using the 'strict equality' operator

We are going to complete a function that takes in two scalar (boolean, number, or string) parameters. Your function should create a variable and assign it to the result of comparing the two input parameters using the `===` operator, then return that variable. Below are examples of the code running, assuming that you will have completed the described function: `areEqual`.

```javascript
var outputTrue = areEqual("happiness", "happiness");
console.log('should be true:', outputTrue);

var outputFalse = areEqual(0, false);
console.log('should be false:', outputFalse);
```

```javascript
function areEqual(param_1, param_2) {
  // create a result variable
  // assign it to a comparison between param_1 and param_2 using "equal to" operator
  // return the result variable
  var result = param_1 === param_2;
  return result;
}
```

#### Not equal to | Using the 'strict not equality' operator

We are going to complete a function that takes in two scalar (boolean, number, or string) parameters. Your function should create a variable and assign it to the result of comparing the two input parameters using the `!==` operator, then return that variable. Below are examples of the code running, assuming that you will have completed the described function: `areNotEqual`.

```javascript
var outputTrue = areNotEqual("happiness", "sadness");
console.log('should be true:', outputTrue);

var outputFalse = areNotEqual(7, 3 + 4);
console.log('should be false:', outputFalse);
```

```javascript
function areNotEqual(param_1, param_2) {
  // create a result variable
  // assign it to a comparison between param_1 and param_2 using "not equal to" operator
  // return the result variable
  var result = param_1 !== param_2;
  return result;
}
```

### Working with Numbers

#### Addition | Using the `+` operator with numbers

We are going to complete a function that takes in two number parameters, and returns their sum when added together. Your function should create a variable and assign it to the result of adding the two input parameters together using the + operator, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `getSum`.

```javascript
var resultSum = getSum(4, 10);
console.log('should be 14:', resultSum);
```

```javascript
function getSum(num1, num2) {
  // create a result variable,
  // assign it to num1 and num2 added together
  // return the result variable
  var r = num1 + num2;
  return r;
}
```

#### Subtraction | Using the `-` operator with numbers

We are going to complete a function that takes in two number parameters (num1, num2), and returns their difference when num2 is subtracted from num1. Your function should create a variable and assign it to the result of subtracting num2 from num1 using the - operator, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `getDifference`.

```javascript
var resultDiff = getDifference(37, 19);
console.log('should be 18:', resultDiff);
```

```javascript
function getDifference(num1, num2) {
  // create a result variable,
  // assign it to num1 minus num2
  // return the result variable
  var r = num1 - num2;
  return r;
}
```

#### Multiplication | Using the `*` operator with numbers

We are going to complete a function that takes in two number parameters, and returns their product when multiplied together. Your function should create a variable and assign it to the result of multiplying the number parameters together using the * operator, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `getProduct`.

```javascript
var resultProduct = getProduct(9, 4);
console.log('should be 36:', resultProduct);
```

```javascript
function getProduct(num1, num2) {
  // create a result variable,
  // assign it to num1 times num2
  // return the result variable
  var r = num1 * num2;
  return r;
}
```

#### Division | Using the `/` operator with numbers

We are going to complete a function that takes in two number parameters (num1, num2), and returns the result of num1 divided by num2. Your function should create a variable and assign it to the result of dividing num1 by num2 using the / operator, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `getQuotient`.

```javascript
var resultQuotient = getQuotient(20, 4);
console.log('should be 5:', resultQuotient);
```

```javascript
function getQuotient(num1, num2) {
  // create a result variable,
  // assign it to num1 divided by num2
  // return the result variable
  var  r = num1 / num2;
  return r;
}
```

#### Exponent | Using the `**` operator with numbers

We are going to complete a function that takes in two number parameters (num1, num2), and returns the result of raising num1 to the num2 power. Your function should create a variable and assign it to the result of raising num1 to the num2 power using the ** operator, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `getPower`.

```javascript
var resultPower = getPower(3, 4);
console.log('should be 81:', resultPower);
```

```javascript
function getPower(num1, num2) {
  // create a result variable,
  // assign it to num1 raised to the num2 power
  // return the result variable
  var r = num1 ** num2;
  return r;
}
```

#### Modulo | Using the `%` operator with numbers

We are going to complete a function that takes in two number parameters (num1, num2), and returns the remainder after dividing num1 by num2. Your function should create a variable and assign it to the remainder after dividing num1 by num2 using the `%` operator, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `getRemainder`.

```javascript
var resultRemainder = getRemainder(21, 6);
console.log('should be 3:', resultRemainder);
```

```javascript
function getRemainder(num1, num2) {
  // create a result variable,
  // assign it to remainder after dividing num1 by num2
  // return the result variable
  var r = num1 % num2;
  return r;
}
```

#### Plus-equals | Using the `+=` operator

We are going to complete a function that takes in two number parameters (base, incrementer), and returns the result of incrementing the base by the incrementer. Your function should reassign base to the result of incrementing base by incrementer using the `+=` operator, then return base. Below is an example of the code running, assuming that you will have completed the described function: `increment`.

```javascript
var resultIncremented = increment(11, 5);
console.log('should be 16:', resultIncremented);
```

```javascript
function increment(base, incrementer) {
  // reassign base to result of incrementing base by incrementer
  // return base
  var r  = base += incrementer;
  return r;
}
```

#### Minus-equals | Using the `-=` operator

We are going to complete a function that takes in two number parameters (base, decrementer), and returns the result of decrementing the base by the decrementer. Your function should reassign base to the result of decrementing base by decrementer using the `-=` operator, then return base. Below is an example of the code running, assuming that you will have completed the described function: `decrement`.

```javascript
var resultDecremented = decrement(17, 5);
console.log('should be 12:', resultDecremented);
```

```javascript
function decrement(base, decrementer) {
  // reassign base to result of decrementing base by decrementer
  // return base
  var r = base -= decrementer;
  return r;
}
```

#### Times-equals | Using the `*=` operator

We are going to complete a function that takes in two number parameters (base, multiplier), and returns the result of reassigning the base to be the base multiplied by the multiplier. Your function should reassign base to the result of multipling base by multiplier using the `*=` operator, then return base. Below is an example of the code running, assuming that you will have completed the described function: `applyTimesEquals`.

```javascript
var resultMultiplied = applyTimesEquals(3, 5);
console.log('should be 15:', resultMultiplied);
```

```javascript
function applyTimesEquals(base, multiplier) {
  // reassign base to result of multiplying base by multiplier
  // return base
  var r = base *= multiplier;
  return r;
}
```

#### Divide-equals | Using the `/=` operator

We are going to complete a function that takes in two number parameters (base, divider), and returns the result of reassigning the base to be the base divided by the divider. Your function should reassign base to the result of dividing base by divider using the `/=` operator, then return base. Below is an example of the code running, assuming that you will have completed the described function: `applyDivideEquals`.

```javascript
var resultDivided = applyDivideEquals(56, 7);
console.log('should be 8:', resultDivided);
```

```javascript
function applyDivideEquals(base, divider) {
  // reassign base to result of dividing base by divider
  // return base
  var r = base /= divider;
  return r;
}
```

#### Absolute Value | Using the `Math.abs()` method

We are going to complete a function that takes in one number parameter, and returns the absolute value of said parameter. Your function should create a variable and assign it to the result of applying the `Math.abs()` method to the input parameter, then return that variable. Below are examples of the code running, assuming that you will have completed the described function: `getAbsoluteValue`.

```javascript
var result1 = getAbsoluteValue(-56);
console.log('should be 56:', result1);

var result2 = getAbsoluteValue(127);
console.log('should be 127:', result2);
```

```javascript
function getAbsoluteValue(num) {
  // create a result variable
  // assign it to absolutely value of input num
  // return result
  var r = Math.abs(num);
  return r;
}
```

#### Rounding Up and Rounding Down | Using the `Math.floor()` method

We are going to complete a function that takes in one number parameter, and returns the result of rounding the number down. Your function should create a variable and assign it to the result of applying the `Math.floor()` method to the input parameter, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `roundDown`.

```javascript
var roundedDown = roundDown(6.8);
console.log('should be 6:', roundedDown);
```

```javascript
function roundDown(num) {
  // create a result variable
  // assign it to input, rounded down
  // return result
  var r = Math.floor(num);
  return r;
}
```

#### #### Rounding Up and Rounding Down | Using the `Math.ceil()` method

We are going to complete a function that takes in one number parameter, and returns the result of rounding the number up. Your function should create a variable and assign it to the result of applying the `Math.ceil()` method to the input parameter, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `roundUp`.

```javascript
var roundedUp = roundUp(16.8);
console.log('should be 17:', roundedUp);
```

```javascript
function roundUp(num) {
  // create a result variable
  // assign it to input, rounded up
  // return result
   var r = Math.ceil(num);
  return r;
}
```

#### Parsing an Integer or a Float from a String | Using the `Number.parseInt()` method

We are going to complete a function that takes in one string parameter, representing an integer, and returns the result of parsing an integer from the input. Your function should create a variable and assign it to the result of applying the `Number.parseInt()` method to the input parameter, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `applyParseInt`.

```javascript
var parsedInteger = applyParseInt("23");
console.log('should be 23:', parsedInteger);
```

```javascript
function applyParseInt(numString) {
  // create a result variable
  // assign it to parsed integer from input string
  // return result
  var r = Number.parseInt(numString);
  return r;
}
```

#### Parsing an Integer or a Float from a String | Using the `Number.parseFloat()` method

We are going to complete a function that takes in one string parameter, representing a float (decimal), and returns the result of parsing a float from the input. Your function should create a variable and assign it to the result of applying the `Number.parseFloat()` method to the input parameter, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `applyParseFloat`.

```javascript
var parsedFloat = applyParseFloat("101.78");
console.log('should be 101.78:', parsedFloat);
```

```javascript
function applyParseFloat(numString) {
  // create a result variable
  // assign it to parsed float from input string
  // return result
  var r = Number.parseFloat(numString);
  return r;
}
```

#### Generate a Random Number | Using the `Math.random()` method

We are going to complete a function that takes in two number parameters, representing the lower and upper bounds for a random number to be generated, and returns a randomly generated number within the described bounds. Your function should create a variable and assign it to the result of generating a random number using the `Math.random()` method, along with the formula described above, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `generateRandomNumber`.

```javascript
var randomNumber = generateRandomNumber(1, 10);
console.log('should be between 1 and 10:', randomNumber);
```

```javascript
function generateRandomNumber(min, max) {
  // create a result variable
  // assign it to formula for random number between min and max
  // return result
  var r = Math.random() * (max - min) + min;
  return r;
}
```

#### Greater than | Using the `>` operator

We are going to complete a function that takes in two number parameters (num1, num2), and returns whether num1 is greater than num2. Your function should create a variable and assign it to the result of comparing num1 to num2 using the > operator, then return that variable. Below are examples of the code running, assuming that you will have completed the described function: `applyGreaterThan`.

```javascript
var trueGreaterThanResult = applyGreaterThan(101, 10);
console.log('should be true:', trueGreaterThanResult);

var falseGreaterThanResult = applyGreaterThan(-13, 2);
console.log('should be false:', falseGreaterThanResult);
```

```javascript
function applyGreaterThan(num1, num2) {
  // create a result variable
  // assign it expression comparing if num1 is greater than num2
  // return result
  var r = num1 > num2;
  return r;
}
```

#### Less than | Using the `<=` operator

We are going to complete a function that takes in two number parameters (num1, num2), and returns whether num1 is less than or equal to num2. Your function should create a variable and assign it to the result of comparing num1 to num2 using the <= operator, then return that variable. Below are examples of the code running, assuming that you will have completed the described function: `applyLessThanOrEqualTo`.

```javascript
var trueLessThanOrEqualToResult = applyLessThanOrEqualTo(11, 110);
console.log('should be true:', trueLessThanOrEqualToResult);

var falseLessThanOrEqualToResult = applyLessThanOrEqualTo(-13, -21);
console.log('should be false:', falseLessThanOrEqualToResult);
```

```javascript
function applyLessThanOrEqualTo(num1, num2) {
  // create a result variable
  // assign it expression comparing if num1 is less than or equal num2
  // return result
  var r = num1 <= num2;
  return r;
}
```

### Working with Strings

#### Creating a String

We are going to complete a function that takes no parameters, and returns a newly created string. Your function should create a variable and assign it to a new string, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `createString`.

```javascript
var resultString = createString();
console.log('should be a string type:', typeof resultString);
```

```javascript
function createString() {
  // create a result variable,
  // assign it to a new string
  // return the result variable
  var r = "hello";
  return r;
}
```

#### Accessing a Character in a String

We are going to complete a function that takes two parameters, a string and a numerical index, and returns the character in the string located at the numerical index. Your function should create a variable and assign it to an expression which accesses the character located at the numerical index, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `accessACharacter`.

```javascript
var resultCharacter = accessACharacter('Computer', 3);
console.log('should be "p":', resultCharacter);
```

```javascript
function accessACharacter(string, index) {
  // create a result variable,
  // assign it to an expression that accesses the character within string at the index
  // return the result variable
  var r = string[index];
  return r;
}
```

#### Reassigning a String's Value

We are going to complete a function that takes one string parameter, and reassigns the input parameter to be "reassigned", then returns that input. Your function should not create any new variables and should reassign the input to the string "reassigned", then return the input parameter. Below are examples of the code running, assuming that you will have completed the described function: `reassignAString`.

```javascript
var resultString1 = reassignAString('Computer Science');
console.log('should be "reassigned":', resultString1);

var resultString2 = reassignAString('Software Engineering');
console.log('should also be "reassigned":', resultString2);
```

```javascript
function reassignAString(string) {
  // reassign input string to described string
  // return the input string
  var r = 'reassigned';
  return r;
}
```

#### Concatenate two strings

We are going to complete a function that takes in two parameters, both will be strings, and returns the two strings concatenated. Your function should create a new variable, assign it to an expression which will add together or concatenate the input strings, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `addTogetherTwoStrings`.

```javascript
var resultString1 = addTogetherTwoStrings('Comp', 'uter');
console.log('should be "Computer":', resultString1);

var resultString2 = addTogetherTwoStrings('Engin', 'eering');
console.log('should also be "Engineering":', resultString2);
```

```javascript
function addTogetherTwoStrings(string1, string2) {
  // create a result variable
  // assign it to an expression which adds together string1 and string2
  // return the result variable
  var r = string1 + string2;
  return r;
}
```

#### Concatenate two strings into a full name

We are going to complete a function that takes in two parameters, both will be strings, representing a first name and a last name, and returns a full name string. Your function should create a new variable, assign it to an expression which will add together or concatenate the first and last name strings, with a space in between, then return the that variable. Below is an example of the code running, assuming that you will have completed the described function: `createFullName`.

```javascript
var resultFullName1 = createFullName("Duevyn", "Cooke");
console.log("should log Duevyn Cooke:", resultFullName1);

var resultFullName2 = createFullName("Ada", "Lovelace");
console.log("should log Ada Lovelace:", resultFullName2);
```

```javascript
function createFullName(firstName, lastName) {
  // create a fullName variable
  // assign it to an expression adding first and last name with a space in between
  // return the fullName variable
  var r = firstName + " " + lastName;
  return r;
}
```

#### Interpolate a Variable's value into String | String Interpolation

We are going to complete a function that takes in two parameters, both will be strings (activity, dayOfTheWeek), and returns a message based on the inputs. Your function should create a new variable, assign it to an expression which will interpolate the parameters into a message (described below), then return that variable. Below are examples of the code running, assuming that you will have completed the described function: `interpolateAString`.

```javascript
var resultMessage1 = interpolateAString('hiking', 'Tuesday');
console.log("should log 'We will go hiking on Tuesday.':", resultMessage1);

var resultMessage2 = interpolateAString('dancing', 'Friday');
console.log("should log 'We will go dancing on Friday.':", resultMessage2);
```

```javascript
function interpolateAString(activity, dayOfTheWeek) {
  // create a result variable
  // assign it to an expression which interpolates the input parameters into the described message
  // return the result variable
  var r = 'We will go ' + activity + ' on ' + dayOfTheWeek + '.';
  return r;
}
```

#### Get length of string

We are going to complete a function that takes in one parameter, a string, and returns the length of that string. Your function should create a variable and assign it to the length of the input string using the `.length` property, and return that variable. Below are examples of the code running, assuming that you will have completed the described function: `getStringLength`.

```javascript
var resultLength1 = getStringLength('Apple');
console.log('should log 5:', resultLength1);

var resultLength2 = getStringLength('Microsoft');
console.log('should log 9:', resultLength2);
```

```javascript
function getStringLength(string) {
  // create a length variable
  // assign it to the length of the string
  // return the length variable
  var r = string.length;
  return r;
}
```

#### Get last character of string

We are going to complete a function that takes in one parameter, a string, and returns the input string's last character. Your function should determine the length of the input string minus 1, and assign it to a lastIndex variable. Your function should also create a lastCharacter variable and assign it to an expression which uses lastIndex to access the last character in the string, and return the lastCharacter variable. Below are examples of the code running, assuming that you will have completed the described function: getLastCharacter.

```javascript
var resultLastCharacter1 = getLastCharacter('Banana');
console.log('should log "a":', resultLastCharacter1);

var resultLastCharacter2 = getLastCharacter('Macrofirm');
console.log('should log "m":', resultLastCharacter2);
```

```javascript
function getLastCharacter(string) {
  // create a lastIndex variable
  // assign it to the last index in the string
  // create a lastCharacter variable
  // assign it to the last character in the string (make use of lastIndex)
  // return the lastCharacter variable
  var r = string[string.length - 1]''
  return r'
}
```

#### Apply substring Method

We are going to complete a function that takes in three parameters (string, start, end -> where start and end are numerical indexes), and returns a portion of the string from before start, up to, but not including, end. Your function should create a subString variable and assign it to a call of the substring() method on the string, starting from before start, up to, but not including, end, and return the subString variable. Below are examples of the code running, assuming that you will have completed the described function: `applySubString`.

```javascript
var string1 = 'Queue';
var resultSubString1 = applySubString(string1, 1, 4);
console.log('should log "ueu":', resultSubString1);

var string2 = 'Stack Trace';
var resultSubString2 = applySubString(string2, 2, 10);
console.log('should log "ack Trac":', resultSubString2);
```

```javascript
function applySubString(string, start, end) {
  // create a subString variable
  // assign it to a portion of the string from before start, up to, but not including end
  // return the subString variable
  var r = string.substring(start, end);
  return r;
}
```

#### Apply indexOf Method

We are going to complete a function that takes in two parameters (string, subString), and returns the index of the string where the subString can be found. Your function should create an index variable and assign it to a call of the indexOf() method on the string, and passing subString as an argument, and return the index variable. Below are examples of the code running, assuming that you will have completed the described function: `applyIndexOf`.

```javascript
var string1 = 'Quicksort';
var subString1 = 'sort';
var resultIndex1 = applyIndexOf(string1, subString1);
console.log('should log 5:', resultIndex1);

var string2 = 'size,color,cut,price';
var subString2 = 'cut';
var resultIndex2 = applyIndexOf(string2, subString2);
console.log('should log 11:', resultIndex2);
```

```javascript
function applyIndexOf(string, subString) {
  // create an index variable
  // assign it to the index inside of string where subString can first be found
  // return the index variable
  var r = string.indexOf(subString);
  return r;
}
```

#### Apply toString Method

We are going to complete a function that takes in one parameter, and returns a string version of that parameter. Your function should create a stringVersion variable and assign it to a call of the toString() method on the input parameter, and return the stringVersion variable. Below are examples of the code running, assuming that you will have completed the described function: `applyToString`.

```javascript
var input1 = 9374;
var resultString1 = applyToString(input1);
console.log('should log "9374":', resultString1);
console.log('type should be "string":', typeof resultString1);

var input2 = false;
var resultString2 = applyToString(input2);
console.log('should log "false":', resultString2);
console.log('type should be "string":', typeof resultString2);
```

```javascript
function applyToString(param) {
  // create a stringVersion variable
  // assign it to the string version of the input param
  // return the stringVersion variable
  var r = param.toString();
  return r;
}
```

#### Using Escape Characters

We are going to complete a function that takes in three string parameters (the first, second, and third lines of a haiku), and returns a string that when logged to the console, outputs the haiku in traditional format - see example above. Your function should create a haiku variable and assign it to an expression which will create one "printable onto three lines" string out of the three input strings, and return the haiku variable. Below are examples of the code running, assuming that you will have completed the described function: `generateHaiku`.

```javascript
var resultHaiku1 = generateHaiku('In the twilight rain', 'these brilliant-hued hibiscus -', 'A lovely sunset.');
console.log('should log formatted haiku:\n', resultHaiku1);

var resultHaiku2 = generateHaiku('The lamp once out', 'Moves west, flowers\' shadows', 'Creep eastward.');
console.log('should also log formatted haiku:\n', resultHaiku2);
```

```javascript
function generateHaiku(firstLine, secondLine, thirdLine) {
  // create a haiku variable
  // assign it to an expression involving the input lines, such that they format correct when the return value is logged to the console
  // return the haiku variable
  var r = firstLine + "\n" + secondLine + "\n" + thirdLine
  return r 
}
```

### Working with Arrays

#### Creating an Array

We are going to complete a function that takes no parameters, and returns a newly created array. Your function should create a variable and assign it to a new array, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `createArray`.

```javascript
var resultArray = createArray();
console.log('should be an array:', Array.isArray(resultArray));
```

```javascript
function createArray() {
  // create a result variable,
  // assign it to a new array
  // return the result variable
  var r = ["a", 5, ["b"]];
  return r;
}
```

#### Accessing an Element in an Array

We are going to complete a function that takes two parameters, an array and a numerical index, and returns the element in the array located at the numerical index. Your function should create a variable and assign it to an expression which accesses the element located at the numerical index, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: accessAnElement.

```javascript
var resultElement = accessAnElement(['Computer', 'Mouse', 'Ethernet Cable'], 1);
console.log('should be "Mouse":', resultElement);
```

```javascript
function accessAnElement(array, index) {
  // create a result variable,
  // assign it to an expression that accesses the element within array at the index
  // return the result variable
  var  r = array[index];
  return r;
}
```

#### Reassigning an Element in an Array

We are going to complete a function that takes three parameters, an array, a numerical index, a newValue, and returns the array after performing a reassignment. Your function should reassign the element within the array, located at the numerical index, to the new input value, and should then return the newly changed array. Below is an example of the code running, assuming that you will have completed the described function: `reassignAnElement`.

```javascript
var resultArray = reassignAnElement(['desk', 'lamp', 'chewtoy'], 2, 'textbook');
console.log('should replace "chewtoy" with "textbook":', resultArray);
```

```javascript
function reassignAnElement(array, index, newValue) {
  // reassign the value in the array, located at the index, to the newValue parameter
  // return the input array
  array[index] = newValue;
  return array;
}
```

#### Get length of array

We are going to complete a function that takes in one parameter, an array, and returns the length of that array. Your function should create a variable and assign it to the length of the input array using the .length property, and return that variable. Below are examples of the code running, assuming that you will have completed the described function: `getArrayLength`.

```javascript
var resultLength1 = getArrayLength([1, 3, 4, 5, 7]);
console.log('should log 5:', resultLength1);

var resultLength2 = getArrayLength(['a', 'b', 'c', 'd']);
console.log('should log 4:', resultLength2);
```

```javascript
function getArrayLength(array) {
  // create a length variable
  // assign it to the length of the array
  // return the length variable
  var r = array.length;
  return r;
}
```

#### Get last element of array

We are going to complete a function that takes in one parameter, an array, and returns the input array's last element. Your function should determine the length of the input array minus 1, and assign it to a lastIndex variable. Your function should also create a lastElement variable and assign it to an expression which uses lastIndex to access the last element in the array, and return the lastElement variable. Below are examples of the code running, assuming that you will have completed the described function: ·getLastElement·.

```javascript
var resultLastElement1 = getLastElement([1, 2, "buckle", "my", "shoe"]);
console.log('should log "shoe":', resultLastElement1);

var resultLastElement2 = getLastElement([3, 4, "shut", "the", "door"]);
console.log('should log "door":', resultLastElement2);
```

```javascript
function getLastElement(array) {
  // create a lastIndex variable
  // assign it to the last index in the array
  // create a lastElement variable
  // assign it to the last element in the string (make use of lastIndex)
  // return the lastElement variable
  var index = array.length - 1;
  var r  = array[index];
  return r;
}
```

#### Adding an Element to the back of an Array | Using .push()

We are going to complete a function that takes in two parameters, an array and an element, adds the element to the end of the array, and returns the array. Your function should use the `.push()` method to add the input element to the end of the input array, then return that array. Below are examples of the code running, assuming that you will have completed the described function: `applyPush`.

```javascript
var resultArray1 = applyPush([1, 17, 29], 34);
console.log('should log [1, 17, 29, 34]:', resultArray1);

var resultArray2 = applyPush(['abc', 'def'], 'ghi');
console.log('should log ["abc", "def", "ghi"]:', resultArray2);
```

#### Removing an Element from the back of an Array | Using .pop()

We are going to complete a function that takes in one parameter, an array, removes the last element from the back of the array, and returns the removed element. Your function should create a popped variable, assign it to an expression using the `.pop()` method to remove the last element from the array, then return that popped variable. Below are examples of the code running, assuming that you will have completed the described function: `applyPop`.

```javascript
var resultElement1 = applyPop([1, 171, 129]);
console.log('should log 129:', resultElement1);

var resultElement2 = applyPop(['islands', 'peninsulas', 'pacific']);
console.log('should log pacific:', resultElement2);
```

```javascript
function applyPop(array) {
  // create a popped variable
  // assign it to an expression removing the last element from the array
  // return the popped variable
  var r = array.pop();
  return r;
}
```

#### Add an Element to the front of an Array | Using .unshift()

We are going to complete a function that takes in two parameters, an array and an element, adds the element to the front of the array, and returns the array. Your function should use the `.unshift()` method to add the input element to the front of the input array, then return that array. Below are examples of the code running, assuming that you will have completed the described function: `applyUnshift`.

```javascript
var resultArray1 = applyUnshift([7, 9, 4], 1);
console.log('should log [1, 7, 9, 4]:', resultArray1);

var resultArray2 = applyUnshift(['ef', 'hi'], 'bc');
console.log('should log ["bc", "ef", "hi"]:', resultArray2);
```

```javascript
function applyUnshift(array, element) {
  // add the element to the front of the array
  // return the array
  array.unshift(element);
  return array;
}
```

#### Removing an Element from the front of an Array | Using .shift()

We are going to complete a function that takes in one parameter, an array, removes the first element from the front of the array, and returns the removed element. Your function should create a shifted variable, assign it to an expression using the `.shift()` method to remove the first element from the array, then return that shifted variable. Below are examples of the code running, assuming that you will have completed the described function: `applyShift`.

```javascript
var resultElement1 = applyShift([1, 171, 129]);
console.log('should log 1:', resultElement1);

var resultElement2 = applyShift(['islands', 'peninsulas', 'pacific']);
console.log('should log islands:', resultElement2);
```

```javascript
function applyShift(array) {
  // create a shifted variable
  // assign it to an expression removing the first element from the array
  // return the shifted variable
  var r = array.shift();
  return r;
}
```

#### Adding an Element in General | Using .splice() 

We are going to complete a function that takes in three parameters, an array, an index, and an element, adds the element to the index of the array, without replacing any of the existing elements, and returns the array. Your function should use the `.splice()` method to add the input element to the input array, at the given index, and without replacing any of the existing elements, then returns the array. Below are examples of the code running, assuming that you will have completed the described function: `addAnElementInGeneral`.

```javascript
var resultArray1 = addAnElementInGeneral([7, 9, 10], 1, 8);
console.log('should log [7, 8 , 9, 10]:', resultArray1);

var resultArray2 = addAnElementInGeneral(['q', 'r', 't'], 2, 's');
console.log('should log ["q", "r", "s", "t"]:', resultArray2);
```

```javascript
function addAnElementInGeneral(array, index, element) {
  // add the element to the array at the index given
  // (be sure not to replace any existing elements)
  // return the array
  array.splice(index, 0, element);
  return array;
}
```



