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

#### Removing an Element in General | Using .splice()

We are going to complete a function that takes in two parameters, an array and an index, removes the element from the index of the array, and returns the array. Your function should use the `.splice()` method to remove the element from the input array, at the given index, then return the array. Below are examples of the code running, assuming that you will have completed the described function: `removeAnElementInGeneral`.

```javascript
var resultArray1 = removeAnElementInGeneral([8, 9, 10, 'bad entry', 11], 3);
console.log('should log [8, 9, 10, 11]:', resultArray1);

var resultArray2 = removeAnElementInGeneral(['one', 'two', 452, 'three'], 2);
console.log('should log ["one", "two", "three"]:', resultArray2);
```

```javascript
function removeAnElementInGeneral(array, index) {
  // remove the element from the array at the index given
  // return the array
  array.splice(index,1);
  return array;
}
```

#### Removing and Adding Elements in General | Using .splice()

We are going to complete a function that takes in four parameters, an array, an index, and two new elements, removes 2 elements, beginning at the index, adds the two new elements, and returns the array. Your function should use the `.splice()` method to remove two elements from the input array, at the given index, adds the two new elements in their place, then return the array. Below are examples of the code running, assuming that you will have completed the described function: `applySplice`.

```javascript
var resultArray1 = applySplice([8, 9, 10, 'bad entry1', 'bad entry2', 13], 3, 11, 12);
console.log('should log [8, 9, 10, 11, 12, 13]:', resultArray1);

var resultArray2 = applySplice(['one', 'two', 452, 672, 'five'], 2, 'three', 'four');
console.log('should log ["one", "two", "three", "four", "five"]:', resultArray2);
```

```javascript
function applySplice(array, index, item1, item2) {
  // remove two elements from the array at the index given, and adds item1 and item2 in their place
  // return the array
  array.splice(index,2,item1,item2);
  return array;
}
```

#### Determining if a value is an Array | Using Array.isArray()

We are going to complete a function that takes in one parameter, possibly an array, and returns whether the input in an array or not. Your function should create a variable, assign it to an expression that tells whether the input parameter is an array or not, using the Array.isArray() method, then return that variable. Below are examples of the code running, assuming that you will have completed the described function: `isAnArray`.

```javascript
var resultBoolean1 = isAnArray([1, 2, 3]);
console.log('should log true:', resultBoolean1);

var resultBoolean2 = isAnArray({name: 'Tom', friend: 'Jerry'});
console.log('should log false:', resultBoolean2);
```

```javascript
function isAnArray(input) {
  // create a result variable
  // assign it to a call to the applicable method
  // return the result variable
  var r = Array.isArray(input);
  return r;
}
```

#### Slicing a portion of an Array | Using .slice()

We are going to complete a function that takes in three parameters, an array and two integer indexes (start, end), and returns a portion of the array from before the start index up to, but not including, the end index. Your function should create a sliceOfArray variable and assign it to a call to the slice method on the array, starting from before start, up to, but not including, end, and return the sliceOfArray variable. Below are examples of the code running, assuming that you will have completed the described function: `applySlice`.

```javascript
var array1 = ['Q', 'u', 'e', 'u', 'e'];
var resultOfSlice1 = applySlice(array1, 1, 4);
console.log('should log ["u", "e", "u"]:', resultOfSlice1);

var array2 = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
var resultOfSlice2 = applySlice(array2, 2, 8);
console.log('should log [2, 3, 4, 5, 6, 7]:', resultOfSlice2);
```

```javascript
function applySlice(array, start, end) {
  // create a sliceOfArray variable
  // assign it to a portion of the array from before start, up to, but not including end
  // return the sliceOfArray variable
  var r = array.slice(start,end);
  return r;
}
```

#### Using .slice() to make a copy

We are going to complete a function that takes in one array parameter, and returns a copy of the array. Your function should create a copyOfArray variable and assign it to a call to the slice method on the array which will make a copy, and return the copyOfArray variable. Below are examples of the code running, assuming that you will have completed the described function: `makeACopy`.

```javascript
var array1 = ['Q', 'u', 'e', 'u', 'e'];
var resultCopy1 = makeACopy(array1);
console.log('should log ["Q", "u", "e", "u", "e"]:', resultCopy1);

var array2 = [0, 1, 2, 3, 4];
var resultCopy2 = makeACopy(array2);
```

```javascript
function makeACopy(array) {
  // create a copyOfArray variable
  // assign it to a copy of the array
  // return the copyOfArray variable
  var r = array.slice();
  return r;
}
```

#### Adding the contents of an Array to another Array | Using .concat()

We are going to complete a function that takes in two array parameters, and returns an array containing all of the elements of the two input arrays. Your function should create a concattedArray variable and assign it to a call to the concat method on the input array, applied to the other input array, and return the concattedArray variable. Below are examples of the code running, assuming that you will have completed the described function: `applyConcat`.

```javascript
var array1 = ['a', 'b', 'c'];
var array2 = ['d', 'e', 'f']
var resultConcat1 = applyConcat(array1, array2);
console.log('should log ["a", "b", "c", "d", "e", "f"]:', resultConcat1);

var array3 = [1, 2, 3];
var array4 = [4, 5, 6];
var resultConcat2 = applyConcat(array3, array4);
console.log('should log [1, 2, 3, 4, 5, 6]:', resultConcat2);
```

```javascript
function applyConcat(array1, array2) {
  // create a concattedArray variable
  // assign it to the contents of both array1 and array2
  // return the concattedArray variable
  var r = array1.concat(array2);
  return r;
}
```

#### Transforming an Array into a String | Using .join()

We are going to complete a function that takes in one array parameter (elements will be strings), and one string parameter, and returns a string that is the result of joining the elements of the string together, separated by the string parameter. Your function should create a joinedString variable and assign it to a call to the .join() method, and return the joinedString variable. Below are examples of the code running, assuming that you will have completed the described function: `applyJoin`.

```javascript
var resultString1 = applyJoin(['first', 'second', 'third'], '--');
console.log('should log joined string:', resultString1);

var resultString2 = applyJoin(['git', 'commit'], ' ');
console.log('should also log joined string:', resultString2);
```

```javascript
function applyJoin(arrayOfStrings, string) {
  // create a joinedString variable
  // assign it to a string which is all of the strings in the input array separated by the input string
  // return the joinedString variable
  var r = arrayOfStrings.join(string);
  return r;
}
```

#### Transforming a String into an Array Coding | Using .split()

We are going to complete a function that takes in two string parameters (stringToBeSplit, splitter), and returns an array that is the result of splitting the stringToBeSplit parameter on the splitter parameter. Your function should create a splitString variable and assign it to a call to the .split() method, and return the splitString variable. Below are examples of the code running, assuming that you will have completed the described function:  `applySplit`.

```javascript
var resultArray1 = applySplit('first--second--third', '--');
console.log('should log split string:', resultArray1);

var resultArray2 = applySplit('git push origin master', ' ');
console.log('should also log split string:', resultArray2);
```

```javascript
function applySplit(stringToBeSplit, splitter) {
  // create a splitString variable
  // assign it to an array which contains the elements in the stringToBeSplit separated by the splitter
  // return the splitString variable
  var r = stringToBeSplit.split(splitter);
  return r;
}
```

#### Apply indexOf Method to an Array

We are going to complete a function that takes in two parameters (array, element), and returns the index of the array where the element can be found. Your function should create an index variable and assign it to a call of the indexOf() method on the array, and passing element as an argument, and return the index variable. Below are examples of the code running, assuming that you will have completed the described function: `applyIndexOfToArray`.

```javascript
var array1 = ['Quick', 'sort', 'is', 'wild'];
var element1 = 'sort';
var resultIndex1 = applyIndexOfToArray(array1, element1);
console.log('should log 1:', resultIndex1);

var array2 = ['size', 'color', 'cut', 'price'];
var element2 = 'style';
var resultIndex2 = applyIndexOfToArray(array2, element2);
console.log('should log -1:', resultIndex2);
```

```javascript
function applyIndexOfToArray(array, element) {
  // create an index variable
  // assign it to the index inside of array where element can be found
  // return the index variable
  var r = array.indexOf(element);
  return r;
}
```

### Working with Objects

#### Creating an Object 

We are going to complete a function that takes no parameters, and returns a newly created object. Your function should create a variable and assign it to a new object, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `createObject`.

```javascript
var resultObject = createObject();
console.log('should be an object:', typeof resultObject);
console.log('should not be an array:', Array.isArray(resultObject));
```

```javascript
function createObject() {
  // create a result variable,
  // assign it to a new object
  // return the result variable
  var r = {};
  return r;
}
```

#### Accessing a Property in an Object

We are going to complete a function that takes two parameters, an object and a string key, and returns the value for a property in the object located at the string key. Your function should create a variable and assign it to an expression which accesses the value of the property located at the string key, then return that variable. Below is an example of the code running, assuming that you will have completed the described function: `accessAProperty`.

```javascript
var resultValue = accessAProperty({machine: 'Computer', type: 'Macbook', ram: '2 GHz'}, 'ram');
console.log('should be "2 GHz":', resultValue);
```

```javascript
function accessAProperty(object, key) {
  // create a result variable,
  // assign it to an expression that accesses the property in the object located at the key
  // return the result variable
  var r = object[key];
  return r;
}
```

#### Reassigning a Property's Value in an Object

We are going to complete a function that takes three parameters, an object, a string key, and a newValue, and returns the object after performing a reassignment. Your function should reassign the property's value within the object, located at the string key, to the newValue parameter, and should then return the newly changed object. Below is an example of the code running, assuming that you will have completed the described function: `reassignAProperty`.

```javascript
var resultObject = reassignAProperty({name: 'Ramses', favoriteFood: 'chicken', type: 'dog'}, 'favoriteFood', 'goose');
console.log('should replace "chicken" with "goose":', resultObject);
```

```javascript
function reassignAProperty(object, key, newValue) {
  // reassign the property's value in the object, located at the key, to the newValue parameter
  // return the input object
  object[key] = newValue;
  return object;  
}
```

#### Removing a Property from an Object | Using 'delete' 

We are going to complete a function that takes in two parameters, an object and an key, removes the property located at the input key from the object, and returns the object. Your function should use the delete operator to remove the property at the given key from the input object, then return the object. Below are examples of the code running, assuming that you will have completed the described function: `removeAProperty`.

```javascript
var resultObject1 = removeAProperty({q: 9, r: 10, text: 'bad entry'}, 'text');
console.log('should log {q: 9, r: 10}:', resultObject1);

var resultObject2 = removeAProperty({first: 'one', second: 'two', why: 452, third: 'three'}, 'why');
console.log('should log {first: "one", second: "two", third: "three"}:', resultObject2);
```

```javascript
function removeAProperty(object, key) {
  // remove the property at the given key from the object
  // return the object
  delete object[key];
  return object;
}
```

#### Determine if Property is Present

We are going to complete a function that takes in two parameters an object and a key, and returns whether the object has a property at the given key. Your function should create an isPresent variable and assign it to a comparison between the object's value at the given key and undefined, and return the isPresent variable. Below are examples of the code running, assuming that you will have completed the described function: `isPropertyPresent`.

```javascript
var object1 = {
  a: 1,
  b: 2
}
var key1 = 'c';
var result1 = isPropertyPresent(object1, key1);
console.log('should log false:', result1);

var object2 = {
  'size': 'M',
  'color': 'green',
  'cut': 'tapered',
  'price': 30
};
var key2 = 'cut';
var result2 = isPropertyPresent(object2, key2);
console.log('should log true:', result2);
```

```javascript
function isPropertyPresent(object, key) {
  // create an isPresent variable
  // assign it to a comparison between object's value at key and undefined
  // return the isPresent variable
  var isPresent = object[key] !== undefined;
  return isPresent;
}
```

#### Determine if a value is an Object

We are going to complete a function that takes in one parameter, possibly an object, and returns whether the input in an object or not. Your function should create several variables (isObject, isNotAnArray, and isObjectAndNotAnArray). Assign isObject to an application of the typeof operator to the input. Assign isNotAnArray to a call to the Array.isArray() method with the ! operator applied as well. Assign isObjectAndNotAnArray to the two previous variabes combined with the && operator, and return the isObjectAndNotAnArray variable. Below are examples of the code running, assuming that you will have completed the described function: `isAnObject`.

```javascript
var resultBoolean1 = isAnObject([1, 2, 3]);
console.log('should log false:', resultBoolean1);

var resultBoolean2 = isAnObject({name: 'Tom', friend: 'Jerry'});
console.log('should log true:', resultBoolean2);
```

```javascript
function isAnObject(input) {
  // create an isObject variable
  // assign it to whether the input is an object type
  // create an isNotAnArray variable
  // assign it to whether the input is not an array
  // create an isObjectAndNotAnArray variable
  // assign it to a combination of isObject AND isNotAnArray
  // return the isObjectAndNotAnArray variable
  var isObject = typeof input === "object";
  var isNotAnArray = !Array.isArray(input);
  var isObjectAndNotAnArray = isObject && isNotAnArray;
  return isObjectAndNotAnArray;
}
```

#### Generating an array of all keys in an Object | Using Object.keys()

We are going to complete a function that takes in one parameter, an object. Your function should create a keys variable, and assign it to an expression which generates an array of all of the keys in said object by calling `Object.keys()`, then return that keys variable. Below is an example of the code running, assuming that you will have completed the described function: `getAllKeys`.

```javascript
var resultKeys = getAllKeys({firstScore: 12, secondScore: 34, thirdScore: 28});
console.log('should log ["firstScore", "secondScore", "thirdScore"]:', resultKeys);
```

```javascript
function getAllKeys(obj) {
  // create a keys variable
  // assign it to an expression which will generate an array of all of the keys in obj
  // return to the keys variable
  var keys = Object.keys(obj);
  return keys;
}
```

#### Generating an array of all values in an Object | Using Object.values()

We are going to complete a function that takes in one parameter, an object. Your function should create a values variable, and assign it to an expression which generates an array of all of the values in said object by calling `Object.values()`, then return that values variable. Below is an example of the code running, assuming that you will have completed the described function: `getAllValues`.

```javascript
var resultValues = getAllValues({firstScore: 12, secondScore: 34, thirdScore: 28});
console.log('should log [12, 34, 28]:', resultValues);
```

```javascript
function getAllValues(obj) {
  // create a values variable
  // assign it to an expression which will generate an array of all of the values in obj
  // return to the values variable
  var values = Object.values(obj);
  return values;
}
```

### Nested Structures

#### Method applied to a Nested Array | Using .unshift()

We are going to complete a function that takes in three parameters, a nested array of arrays, an index, and an element, then adds the element to the front of the inner array located at the index within the input array of arrays, and returns the array of arrays. Your function should use the `.unshift()` method to add the input element to the front of the inner array located at the given index of the array of arrays, then return that array of arrays. Below are examples of the code running, assuming that you will have completed the described function: `applyUnshiftAgain`.

```javascript
var resultArray1 = applyUnshiftAgain([ [1, 3], [10, 11], [9, 4] ], 1, 5);
console.log('should log [ [1, 3], [5, 10, 11], [9, 4] ]:', resultArray1);

var resultArray2 = applyUnshiftAgain([ ['ag', 'bc'], ['ef', 'hi'] ], 0, 'iq');
console.log('should log [ ["iq", "ag", "bc"], ["ef", "hi"] ]:', resultArray2);
```

```javascript
function applyUnshiftAgain(arrayOfArrays, index, element) {
  // add the element to the front of the inner array within the array of arrays located at the index
  // return the array of arrays
  var innerArray = arrayOfArrays[index];
  innerArray.unshift(element);
  return arrayOfArrays;
}
```

#### Method applied to an Array within an Object | Using Array.isArray() 

We are going to complete a function that takes in two parameters, one value is an object, possibly containing an array, as well as a key in that object, and returns whether the value located at the key is an array or not. Your function should create a variable, assign it to an expression that tells whether the input object's value located at the input key is an array or not, using the `Array.isArray()` method, then return that created variable. Below are examples of the code running, assuming that you will have completed the described function: `isAnArrayAgain`.

```javascript
var resultBoolean1 = isAnArrayAgain({key1: [1, 2, 3], key2: 'gg'}, 'key1');
console.log('should log true:', resultBoolean1);

var resultBoolean2 = isAnArrayAgain({name: 'Tom', friend: 'Jerry'}, 'friend');
console.log('should log false:', resultBoolean2);
```

```javascript
function isAnArrayAgain(inputObj, key) {
  // create a result variable
  // assign it to a call to the applicable method
  // return the result variable
  var result = Array.isArray(inputObj[key]);
  return result;
}
```

#### Method applied to a Nested Object | Using Object.keys()

We are going to complete a function that takes in two parameters, an object and a key. Your function should create a keys variable, and assign it to an expression which generates an array of all of the keys in the nested object located within the input object, by calling `Object.keys()`, then return that keys variable. Below is an example of the code running, assuming that you will have completed the described function: `getAllKeysAgain`.

```javascript
var resultKeys = getAllKeysAgain({firstScore: {part1: 12, part2: 14, part3: 10}, secondScore: 34, thirdScore: 28}, 'firstScore');
console.log('should log ["par1", "part2", "part3"]:', resultKeys);
```

```javascript
function getAllKeysAgain(obj, key) {
  // create a keys variable
  // assign it to an expression which will generate an array of all of the keys located within obj at key
  // return to the keys variable
  var keys = Object.keys(obj[key]);
  return keys;
}
```

#### Operator applied to an Object within an Array | Using 'delete' 

We are going to complete a function that takes in three parameters, an array, an index, and an key, removes the property specified by the input key, located within an object, located at the given index within the input array, and returns the input array. Your function should use the delete operator to remove the property specified by the input key, located within an object, located at the given index within the input array, and returns the input array. Below are examples of the code running, assuming that you will have completed the described function: `removeAPropertyAgain`.

```javascript
var resultObject1 = removeAPropertyAgain([{q: 9, r: 10, text: 'bad entry'}, {a: 1, b: 2}], 0, 'text');
console.log('should log [{q: 9, r: 10}, {a: 1, b: 2}]:', resultObject1);

var resultObject2 = removeAPropertyAgain([{key: 'value'}, {first: 'one', second: 'two', why: 452, third: 'three'}], 1, 'why');
console.log('should log [{key: "value"}, {first: "one", second: "two", third: "three"}]:', resultObject2);
```

```javascript
function removeAPropertyAgain(arrayOfObjects, index, key) {
  // remove the property at the given key from the object at the given index
  // return the input array of objects
  delete arrayOfObjects[index][key];
  return arrayOfObjects;
}
```

## Conditionals

### IF statement

#### IF statement with undefined

We are going to complete a function that takes in one parameter, determines if that parameter is defined, and returns a specific string if it is. Your function should use an `if` statement to determine if the input parameter is defined, and if it is, should return the string 'Input is defined'. Below are examples of the code running, assuming that you will have completed the described function: `isItUndefined`.

```javascript
var result1 = isItUndefined('anything');
console.log('should log "Input is defined":', result1);

var result2 = isItUndefined();
console.log('Should log undefined, because function returned nothing:', result2);
```

```javascript
function isItUndefined(param) {
  // if param is defined (or not undefined)
    // return 'Input is defined'
    if (param !== undefined){
    return 'Input is defined';
    }
}
```

#### IF statement with numbers

We are going to complete a function that takes in two parameters, both numbers representing totals for apples and oranges, determines if there are fewer apples than oranges, and if so, returns a specific string. Your function should use an `if` statement to determine if there are fewer apples than oranges, and if there are, should return the string 'There are fewer apples than oranges'. Below are examples of the code running, assuming that you will have completed the described function: `fewerApples`.

```javascript
var result1 = fewerApples(4, 7);
console.log('should log "There are fewer apples than oranges":', result1);

var result2 = fewerApples(19, 12);
console.log('Should log undefined, because function returned nothing:', result2);
```

```javascript
function fewerApples(apples, oranges) {
  // if there are fewer apples than oranges
    // return 'There are fewer apples than oranges'
    if ( apples < oranges){
    return 'There are fewer apples than oranges';
    }
}
```

#### IF statement with a string

We are going to complete a function that takes in one parameter, a string representing a password, determines if the string is both longer than 4, and less than 15, characters long, and if it is returns a specific string. Your function should use an `if` statement to determine if the input string is both long enough, and not too long, and if it is, should return the string 'Password length is valid'. Below are examples of the code running, assuming that you will have completed the described function: `validLengthPassword`.

```javascript
var result1 = validLengthPassword('passwordyfurdy');
console.log('should log "Password length is valid":', result1);

var result2 = validLengthPassword('pass');
console.log('Should log undefined, because function returned nothing:', result2);

var result3 = validLengthPassword('this is clearly too long of a password');
console.log('Should log undefined, because function returned nothing:', result3);
```

```javascript
function validLengthPassword(password) {
  // if password length is greater than 4 and less than 15
    // return 'Password length is valid'
    if(password.length>4  && password.length < 15){
    return "Password length is valid";    
    }
}
```

#### IF statement with an array

We are going to complete a function that takes in two parameters, an array of agents in the field, and an agent to search for within that array, determines if the agent to search for is present within the array, and if it is, returns a specific string. Your function should use an if statement to determine if the agent to search for is present within the list of agents, and if it is, should return the string '{agentToSearchFor} is present within Agent list', where {agentToSearchFor} has the value of the argument the function is called on. Below are examples of the code running, assuming that you will have completed the described function: `findAgent`.

```javascript
var result1 = findAgent(['001', '005', '007', '009'], '007');
console.log('should log "007 is present within Agent list":', result1);

var result2 = findAgent(['tiny', 'teeny', 'eeny', 'meany'], 'teeny');
console.log('should log "teeny is present within Agent list":', result2);

var result3 = findAgent(['red', 'blue', 'green'], 'orange');
console.log('Should log undefined, because function returned nothing:', result3);
```

```javascript
function findAgent(agentList, agentToSearchFor) {
  // if agentToSearchFor is present within agentList
    // return '{agentToSearchFor} is present within Agent list'
    if (agentList.indexOf(agentToSearchFor) > -1 ){
    return agentToSearchFor + " is present within Agent list";
    }
}
```

#### IF statement with an object

We are going to complete a function that takes in two parameters, an object containing the report totals for various teams, and the string name of a team, and determines if the given team has surpassed their goal of 5 reports, and if they have, returns a specific string. Your function should use an if statement to determine if the team in question has surpassed their goal of 5 reports, and if they have, should return the string '{teamName} has surpassed goal with {number_of_reports_for_team} reports', where {teamName} has the value of the second argument the function is called on, and {number_of_reports_for_team} is the number of reports in the inputted object argument for {teamName}. Below are examples of the code running, assuming that you will have completed the described function: `generateReportSummary`.

```javascript
var result1 = generateReportSummary({a_team: 12, b_team: 7, c_team: 0}, 'b_team');
console.log('should log "b_team has surpassed goal with 7 reports":', result1);

var result2 = generateReportSummary({blue: 18, red: 8, green: 12}, 'blue');
console.log('should log "blue has surpassed goal with 18 reports":', result2);

var result3 = generateReportSummary({gamma: 1, epsilon: 3, alpha: 4, bravo: 17}, 'alpha');
console.log('Should log undefined, because function returned nothing:', result3);
```

```javascript
function generateReportSummary(reportTotals, teamName) {
  // if teamName's report total is greater than 5
    // return '{teamName} has surpassed goal with reports'
    var teamTotal = reportTotals[teamName];
    if(teamTotal > 5){
        return teamName + ' has surpassed goal with ' + teamTotal +' reports';     
    }
}
```

### IF ELSE statements

#### IF ELSE statement with truthy/falsy

HINT: see "truthy vs. falsy" at end of Booleans Operators and Methods Lesson

We are going to complete a function that takes in one parameter, determines if that parameter is truthy or falsy, and returns a specific string for each case. Your function should use an `if else` statement to determine if the input parameter is truthy, and if it is, should return the string 'Input is truthy', or, if the input parameter is falsy, should return the string 'Input is falsy'. Below are examples of the code running, assuming that you will have completed the described function: `isItTruthy`.

```javascript
var result1 = isItTruthy('anything');
console.log('should log "Input is truthy":', result1);

var result2 = isItTruthy();
console.log('should log "Input is falsy":', result2);

var result3 = isItTruthy("");
console.log('should log "Input is falsy":', result3);

var result4 = isItTruthy(false);
console.log('should log "Input is falsy":', result4);
```

```javascript
function isItTruthy(param) {
  // if param is truthy
    // return 'Input is truthy'
  // otherwise
    // return 'Input is falsy'
    if(param){
        return 'Input is truthy';
    } else {
        return 'Input is falsy';
    }
}
```

#### IF ELSE statement with numbers

We are going to complete a function that takes in two parameters, both numbers representing totals for dogs and cats, determines if dogs are more than 8 and cats are fewer than 9, and returns a specific string for each case. Your function should use an if else statement to determine if there are both more than 8 dogs and fewer than 9 cats, and if there are, should return the string 'number of cats and dogs is acceptable', and if not, should return the string 'number of cats or dogs is not acceptable'. Below are examples of the code running, assuming that you will have completed the described function: `balancePets`.

```javascript
var result1 = balancePets(9, 8);
console.log('should log "number of cats and dogs is acceptable":', result1);

var result2 = balancePets(7, 12);
console.log('should log "number of cats or dogs is not acceptable":', result2);

var result3 = balancePets(7, 7);
console.log('should log "number of cats or dogs is not acceptable":', result3);

var result4 = balancePets(5, 14);
console.log('should log "number of cats or dogs is not acceptable":', result4);
```

```javascript
function balancePets(dogs, cats) {
  // if there are more than 8 dogs and fewer than 9 cats
    // return 'number of cats and dogs is acceptable'
  // otherwise
    // return 'number of cats or dogs is not acceptable'
    if (dogs > 9 && cats < 9){
        return 'number of cats and dogs is acceptable';
    } else {
        return 'number of cats or dogs is not acceptable';
    }
}
```

#### IF ELSE statement with a string

We are going to complete a function that takes in one parameter, a string representing a password, determines whether the password is longer than 8 characters, and returns a specific string for each case. Your function should use an `if else` statement to determine if the input string is long enough, and if it is, should return the string 'Password is long enough', and if it is not, should return the string 'Please enter a password of at least 9 characters'. Below are examples of the code running, assuming that you will have completed the described function: `passwordLongEnough`.

```javascript
var result1 = passwordLongEnough('passafassaword');
console.log('should log "Password is long enough":', result1);

var result2 = passwordLongEnough('wordpass');
console.log('Should log "Please enter a password of at least 9 characters":', result2);
```

```javascript
function passwordLongEnough(password) {
  // if password length is greater than 8
    // return 'Password is long enough'
  // otherwise
    // return 'Please enter a password of at least 9 characters'
    if(password.length > 8){
        return 'Password is long enough';
    } else {
        return 'Please enter a password of at least 9 characters';
    }
}
```

#### IF ELSE statement with an array

We are going to complete a function that takes in two parameters, an array of ingredients for a recipe, and an ingredient to search for within that array, determines whether the ingredient to search for is present within the array, and returns a specific string for each case. Your function should use an if else statement to determine if the ingredient to search for is present within the list of ingredients, and if it is, should return the string '{ingredientToSearchFor} is on the list', and if not, should return the string '{ingredientToSearchFor} is not on the list', where {ingredientToSearchFor} has the value of the argument the function is called on. Below are examples of the code running, assuming that you will have completed the described function: `findIngredient`.

```javascript
var result1 = findIngredient(['flour', 'butter', 'sugar', 'eggs'], 'sugar');
console.log('should log "sugar is on the list":', result1);

var result2 = findIngredient(['milk', 'cereal', 'fruit'], 'pop-tarts');
console.log('should log "pop-tarts is not on the list":', result2);
```

```javascript
function findIngredient(ingredientList, ingredientToSearchFor) {
  // if ingredientToSearchFor is present within ingredientList
    // return '{ingredientToSearchFor} is on the list'
  // otherwise
    // return '{ingredientToSearchFor} is not on the list'
    if(ingredientList.indexOf(ingredientToSearchFor) > -1){
        return ingredientToSearchFor + ' is on the list';
    } else {
        return ingredientToSearchFor + ' is not on the list';
    }
}
```

#### IF ELSE statement with an object

We are going to complete a function that takes in one parameter, an object containing the fruit totals for a project, and determines whether the listed total for bananas is greater than 3 and the listed total for strawberries is greater than 10, and returns a specific string for each case. Your function should use an `if else` statement to determine if the totals of bananas and strawberries are sufficient, and if they are, should return the string 'We have enough fruit, with ' + {totalBananas} + ' bananas, and ' + {totalStrawberries} + ' strawberries', where {totalBananas} and {totalStrawberries} are the numbers of each fruit in the fruit totals object. If they are not, your function should return the string 'We do not have enough of both fruits'. Below are examples of the code running, assuming that you will have completed the described function: `measureRequiredFruit`.

```javascript
var result1 = measureRequiredFruit({bananas: 4, strawberries: 12});
console.log('should log "We have enough fruit, with 4 bananas, and 12 strawberries":', result1);

var result2 = measureRequiredFruit({bananas: 5, strawberries: 15});
console.log('should log "We have enough fruit, with 5 bananas, and 15 strawberries":', result2);

var result3 = measureRequiredFruit({bananas: 2, strawberries: 12});
console.log('should log "We do not have enough of both fruits":', result3);

var result4 = measureRequiredFruit({bananas: 5, strawberries: 8});
console.log('should log "We do not have enough of both fruits":', result4);

var result5 = measureRequiredFruit({bananas: 3, strawberries: 9});
console.log('should log "We do not have enough of both fruits":', result5);
```

```javascript
function measureRequiredFruit(fruitTotals) {
  // if there are more than 3 bananas and more than 10 strawberries
    // return 'We have enough fruit, with {totalBananas} bananas, and {totalStrawberries} strawberries'
  // otherwise
    // return 'We do not have enough of both fruits'
    var totalBananas = fruitTotals.bananas;
    var totalStrawberries = fruitTotals.strawberries;
    if (totalBananas > 3 && totalStrawberries >10) {
        return 'We have enough fruit, with ' + totalBananas + ' bananas, and ' + totalStrawberries +' strawberries';
    } else {
        return 'We do not have enough of both fruits';
    }
}
```

### IF ELSE IF statements

#### IF ELSE IF statement (1)

We are going to complete a function that takes in one parameter, a string representing the choice of Player 1 in a game of rock/paper/scissors, and returns a specific string for four different cases. Your function should use an if else if statement to determine which choice the player has made, then should return: 'Player 1 chose rock'; 'Player 1 chose paper'; 'Player 1 chose scissors'; or, 'Player 1 has chosen poorly!', depending upon the value of the input parameter. Below are examples of the code running, assuming that you will have completed the described function: `player1Choice`.

```javascript
var result1 = player1Choice('rock');
console.log('should log "Player 1 chose rock":', result1);

var result2 = player1Choice('paper');
console.log('should log "Player 1 chose paper":', result2);

var result3 = player1Choice('scissors');
console.log('should log "Player 1 chose scissors":', result3);

var result4 = player1Choice('gun');
console.log('should log "Player 1 has chosen poorly!":', result4);
```

```javascript
function player1Choice(choice) {
  // if player1 chose rock
    // return "Player 1 chose rock"
  // otherwise if player1 chose paper
    // return "Player 1 chose paper"
  // otherwise if player1 chose scissors
    // return "Player 1 chose scissors"
  // otherwise
    // return "Player 1 has chosen poorly!"
    if (choice === 'rock'){
        return "Player 1 chose " + choice;
    } else if (choice === 'paper'){
        return "Player 1 chose " + choice;
    } else if (choice === 'scissors'){
         return "Player 1 chose " + choice;
    } else {
        return "Player 1 has chosen poorly!";
    }
}
```

#### IF ELSE IF statement (2)

We are going to complete a function that takes in one parameter, a number called shirtWidth, and returns a specific string for four different cases. Your function should use an if else if statement to determine which size t-shirt is appropriate based on the following conditions: if the shirtWidth is greater than or equal to 20, and less than 30, the function returns 'You should select a size S'; if the shirtWidth is greater than or equal to 30, and less than 40, the function returns 'You should select a size M'; if the shirtWidth is greater than or equal to 40, and less than 50, the function returns 'You should select a size L'. If none of these conditions is met, the function returns 'You should select a different shirt'. Below are examples of the code running, assuming that you will have completed the described function: `selectShirtSize`.

```javascript
var result1 = selectShirtSize(25);
console.log('should log "You should select a size S":', result1);

var result2 = selectShirtSize(32);
console.log('should log "You should select a size M":', result2);

var result3 = selectShirtSize(47);
console.log('should log "You should select a size L":', result3);

var result4 = selectShirtSize(12);
console.log('should log "You should select a different shirt":', result4);

var result5 = selectShirtSize(67);
console.log('should log "You should select a different shirt":', result5);
```

```javascript
function selectShirtSize(choice) {
  // if shirt is greater than or equal 20 and less than 30
    // return 'You should select a size S'
  // otherwise if shirt is greater than or equal to 30 and less than 40
    // return 'You should select a size M'
  // otherwise if shirt is greater than or equal to 40 and less than 50
    // return 'You should select a size L'
  // otherwise
    // return 'You should select a different shirt'
    if (choice >= 20 && choice <30) {
       return 'You should select a size S';
    } else if (choice >= 30 && choice <40){
       return 'You should select a size M';
    } else if (choice >= 40 && choice <50){
       return 'You should select a size L';
    } else {
       return 'You should select a different shirt';
    }
}
```

#### IF ELSE IF statement (3)

We are going to complete a function that takes in three parameters, an object (recipeMinimums) containing required amounts for two ingredients (tomatoes, onions) in a recipe, and then two numbers representing the current stock of those ingredients (stockTomatoes, and stockOnions), and returns a specific string for four different cases. Your function should use an if else if statement to determine the correct output. If both the stock of onions and tomatoes are less than the recipe minimums, your function should return 'We need more tomatoes and more onions'. If the stock of tomatoes is greater than or equal to the recipe minimum, but the stock of onions is less than the recipe minimum, your function should return 'We have enough tomatoes, but need more onions.' If the stock of tomatoes is less than the recipe minimum, but the stock of onions is greater than or equal to the recipe minimum, your function should return 'We have enough onions, but need more tomatoes'. Finally, if the stock of both ingredients is sufficient, your function should return 'We have enough tomatoes and onions. There will be {excessTomatoes} extra tomato, and {excessOnions} extra onion.', where {excessTomatoes} and {excessOnions} are the number of tomatoes and onions in excess of the minimum that the are in stock (e.g. see example above). Below are examples of the code running, assuming that you will have completed the described function: `verifyStock`.

```javascript
var result1 = verifyStock({tomatoes: 3, onions: 7}, 5, 8);
console.log('should log "We have enough tomatoes and onions. There will be 2 extra tomato, and 1 extra onion.":', result1);

var result2 = verifyStock({tomatoes: 5, onions: 1}, 10, 4);
console.log('should log "We have enough tomatoes and onions. There will be 5 extra tomato, and 3 extra onion.":', result2);

var result3 = verifyStock({tomatoes: 2, onions: 4}, 1, 1);
console.log('should log "We need more tomatoes and more onions.":', result3);

var result4 = verifyStock({tomatoes: 4, onions: 2}, 3, 4);
console.log('should log "We have enough onions, but need more tomatoes.":', result4);

var result5 = verifyStock({tomatoes: 10, onions: 6}, 11, 4);
console.log('should log "We have enough tomatoes, but need more onions.":', result5);
```

```javascript
function verifyStock(recipeMinimums, stockTomatoes, stockOnions) {
  // if stock of tomatoes and stock of onions are both less than minimum
    // return 'We need more tomatoes and more onions.'
  // otherwise if stock of tomatoes is less than minimum but stock of onions is sufficient
    // return 'We have enough onions, but need more tomatoes.'
  // otherwise if stock of tomatoes is sufficient but stock of onions is less than minimum
    // return 'We have enough tomatoes, but need more onions.'
  // otherwise
    // return 'We have enough tomatoes and onions. There will be {excessTomatoes} extra tomato, and {excessOnions} extra onion.'
var excessTomatoes = stockTomatoes - recipeMinimums.tomatoes
var excessOnions = stockOnions - recipeMinimums.onions

if (excessTomatoes < 0 && excessOnions < 0){
    return 'We need more tomatoes and more onions.';
} else if (excessTomatoes < 0 && excessOnions >= 0 ){
    return 'We have enough onions, but need more tomatoes.';
} else if (excessTomatoes >= 0 && excessOnions < 0){
    return 'We have enough tomatoes, but need more onions.';
} else { 
    return 'We have enough tomatoes and onions. There will be ' + excessTomatoes + ' extra tomato, and ' + excessOnions + ' extra onion.'; 
}
```

#### Convert Score To Grade

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
var output = convertScoreToGrade(91);
console.log(output); // --> 'A'
```

```javascript
function convertScoreToGrade(score) {
  if (score > 100 || score <0){
      return 'INVALID SCORE';
  } else if (score < 60) {
      return 'F';
  } else if (score < 70) {
      return 'D';
  } else if (score < 80) {
      return 'C';
  } else if (score < 90) {
      return 'B';
  } else {
      return 'A';
  }
}
```

## Loops

### While Loops

#### While loop over a series of numbers

We are going to complete a function that takes two parameters, both will be integers (start, end), and logs to the console, all of the integers starting with start, and ending with end. Your function should use a while loop to log each integer from start, up to and including end, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopASequence`.

```javascript
loopASequence(2, 5);
// console output:
  // 2
  // 3
  // 4
  // 5

loopASequence(3, 7);
// console output:
  // 3
  // 4
  // 5
  // 6
  // 7
```

```javascript
function loopASequence(start, end) {
  // create a loop which runs if start is less than or equal to end
    // log current value of start to console
    // increment value of start
  while (start <= end) {
      console.log(start);
      start++;
  }
}
```

#### While loop over an array

We are going to complete a function that takes one parameter, an array of elements, and logs all of its elements (one at a time) to the console. Your function should use a while loop to log each element from the beginning to the end of the array, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopAnArray`.

```javascript
loopAnArray(['a', 'b', 'c', 'd']);
// console output:
  // a
  // b
  // c
  // d

loopAnArray([1, 2, 3, 4, 5]);
// console output:
  // 1
  // 2
  // 3
  // 4
  // 5
```

```javascript
function loopAnArray(array) {
  // create an index variable
  // create a loop which iterates over the input array
    // log current array element to the console
    // increment value of index variabl
  var index = 0;
  while (index < array.length) {
    var currentVal = array[index];
    console.log(currentVal);
    index++;
  }
}
```

#### While loop over a string

We are going to complete a function that takes one parameter, a string of characters, and logs all of its characters (one at a time) to the console. Your function should use a while loop to log each character from the beginning to the end of the string, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: loopAString.

```javascript
loopAString('nodeJS');
// console output:
  // n
  // o
  // d
  // e
  // J
  // S

loopAString('abcd');
// console output:
  // a
  // b
  // c
  // d
```

```javascript
function loopAString(string) {
  // create an index variable
  // create a loop which iterates over the input string
    // log current string character to the console
    // increment value of index variable
  var i = 0;
  while (i < string.length ) { 
    console.log(string[i]);
    i++;
  }
}
```

### For Loops

#### For loop over a series of numbers

We are going to complete a function that takes two parameters, both will be integers (start, end), and logs to the console, all of the integers starting with start, and ending with end. Your function should use a for loop to log each integer from start, up to and including end, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopASequenceAgain`.

```javascript
loopASequenceAgain(2, 5);
// console output:
  // 2
  // 3
  // 4
  // 5

loopASequenceAgain(3, 7);
  // console output:
    // 3
    // 4
    // 5
    // 6
    // 7
```

```javascript
function loopASequenceAgain(start, end) {
  // create a loop which loops from start to end
    // log current value to console
  for ( value = start; value <= end; value++ ) {
    console.log(value);
  }
}
```

#### For loop over an array

We are going to complete a function that takes one parameter, an array of elements, and logs all of its elements (one at a time) to the console. Your function should use a for loop to log each element from the beginning to the end of the array, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopAnArrayAgain`.

```javascript
loopAnArrayAgain(['a', 'b', 'c', 'd']);
// console output:
  // a
  // b
  // c
  // d

loopAnArrayAgain([1, 2, 3, 4, 5]);
// console output:
  // 1
  // 2
  // 3
  // 4
  // 5
```

```javascript
function loopAnArrayAgain(array) {
  // create a loop which iterates over the input array
    // log current array element to the console
  for ( var i = 0 ; i < array.length ; i++) {
    console.log(array[i]);
  }
}
```

#### For loop over a string

We are going to complete a function that takes one parameter, a string of characters, and logs all of its characters (one at a time) to the console. Your function should use a for loop to log each character from the beginning to the end of the string, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopAStringAgain`.

```javascript
loopAStringAgain('nodeJS');
// console output:
  // n
  // o
  // d
  // e
  // J
  // S

loopAStringAgain('abcd');
// console output:
  // a
  // b
  // c
  // d
```

```javascript
function loopAStringAgain(string) {
  // create a loop which iterates over the input string
    // log current string character to the console
  for (var i = 0; i < string.length; i++) {
    console.log(string[i]);
  }
}
```

#### Loop over every other value

We are going to complete a function that takes one parameter, an array of elements, and logs every other one of its elements, beginning at index 0, to the console. Your function should use a loop to log every other element from the beginning, skipping every other element, until either end of the array, or one shy of the end (depending on odd or even length of the array passed), then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopEveryOther`.

```javascript
loopEveryOther(['a', 'b', 'c', 'd']);
// console output:
  // a
  // c

loopEveryOther([1, 2, 3, 4, 5]);
// console output:
  // 1
  // 3
  // 5
``` 

```javascript
function loopEveryOther(array) {
  // create a loop which iterates over every other element of the input array
    // log every other array element to the console
  for (var i = 0; i < array.length; i += 2) {
    console.log(array[i]);
  }
}
```

#### Loop starting at a specific index

We are going to complete a function that takes two parameters, an array of elements, and an index, and logs every element, beginning at the inputted index (one at a time) to the console. Your function should use a loop to log every element from the inputted index, until the end of the array, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopStartingAtIndex`.

```javascript
loopStartingAtIndex(['a', 'b', 'c', 'd', 'e'], 2);
// console output:
  // c
  // d
  // e

loopStartingAtIndex([1, 2, 3, 4, 5], 3);
// console output:
  // 4
  // 5
```

```javascript
function loopStartingAtIndex(array, index) {
  // create a loop which iterates from index to the end of the input array
    // log current array element to the console
  for (var i = index; i < array.length; i++) {
    console.log(array[i]);
  }
}
```

#### Loop in reverse order

We are going to complete a function that takes one parameter, an array of elements, and logs every element, beginning at the back of the input array and ending at the front of the input array, to the console. Your function should use a loop to log every element from the back of the array, up to the front of the array, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopInReverse`.

```javascript
loopInReverse(['a', 'b', 'c', 'd']);
// console output:
  // d
  // c
  // b
  // a

loopInReverse([1, 2, 3, 4]);
// console output:
  // 4
  // 3
  // 2
  // 1
```

```javascript
function loopInReverse(array) {
  // create a loop which iterates from back to front of the input array
    // log current array element to the console
  for (var i = array.length - 1; i > -1; i--) {
    console.log(array[i]);
  }
}
```

#### Use a 'continue' statement

We are going to complete a function that takes two parameters, an array of elements and an index, and logs every element, except for the element at the input index, to the console. Your function should use a loop to log every element except one at the inputted index, and should also use a continue statement (must use a semi-colon after `continue` for tests to pass) to skip over the value at the inputted index, then return nothing. Your code should NOT use `else`. Below is an example of the code running, assuming that you will have completed the described function: `useContinue`.

```javascript
useContinue(['a', 'b', 'c', 'd'], 1);
// console output:
  // a
  // c
  // d


useContinue([1, 2, 3, 4], 2);
// console output:
  // 1
  // 2
  // 4
```

```javascript
function useContinue(array, index) {
  // create a loop which iterates over the input array
    // if current index is equal to input index
      // use described statement to skip to next iteration of loop (must include semi-colon!)
    // log current array element to the console
  for (var i = 0; i < array.length; i++) {
    if (i === index) {
       continue;
    }
    console.log(array[i]);
  }
}
```

#### Use a 'break' statement

We are going to complete a function that takes two parameters, an array of elements and an index, and logs every element, except those whose index is greater than the input index. Your function should use a loop to log every element up to and including the element located at the input index, and should also use a `break` statement (must use a semi-colon after break for tests to pass) to skip over the values with indexes greater than that of the input index, then return nothing. Your code should NOT use `else`. Below is an example of the code running, assuming that you will have completed the described function: `useBreak`.

```javascript
useBreak(['a', 'b', 'c', 'd', 'e'], 2);
// console output:
  // a
  // b
  // c


useBreak([1, 2, 3, 4, 5, 6], 3);
// console output:
  // 1
  // 2
  // 3
  // 4
```

```javascript
function useBreak(array, index) {
  // create a loop which iterates over the input array
    // if current index is greater than input index
      // use described statement to stop the loop completely (must include semi-colon!)
    // log current array element to the console
  for (var i = 0; i < array.length; i++) {
    if (i > index) {
      break;
    }
    console.log(array[i]);
  }
}
```

### For-in Loops

#### For-in loop over an object (1)

We are going to complete a function that takes one parameter, an object of properties, and logs all of its keys (one at a time) to the console. Your function should use a for-in loop to log each key in the object, then return nothing. DO NOT USE Object.keys() in your solution. Below is an example of the code running, assuming that you will have completed the described function: `loopOverKeys`.

```javascript
loopOverKeys({a: 1, b: 2, c: 3});
// console output:
  // a
  // b
  // c

loopOverKeys({make: 'Ford', model: 'T', year: 1913});
// console output:
  // make
  // model
  // year
```

```javascript
function loopOverKeys(object) {
  // create a loop which iterates over the input object
    // log current key to the console
  for (var currentKey in object){
    console.log(currentKey);
  }
}
```

#### For-in loop over an object (2)

We are going to complete a function that takes one parameter, an object of properties, and logs all of its values (one at a time) to the console. Your function should use a for-in loop to log each value in the object, then return nothing. DO NOT USE Object.values() in your solution. Below is an example of the code running, assuming that you will have completed the described function: `loopOverValues`.

```javascript
loopOverValues({a: 1, b: 2, c: 3});
// console output:
  // 1
  // 2
  // 3

loopOverValues({make: 'Ford', model: 'T', year: 1913});
// console output:
  // Ford
  // T
  // 1913
```

```javascript
function loopOverValues(object) {
  // create a loop which iterates over the input object
    // log current value to the console
  for (var key in object) {
    console.log(object[key]);
  }
}
```

### Nested Loops

#### For loop over an array of arrays

We are going to complete a function that takes one parameter, an array of arrays, and logs all of its elements (log each element in first inner array, start to end, then second inner array, and so on...) to the console. Your function should use a nested `for` loop to log each element from all inner arrays, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopAnArrayOfArrays`.

```javascript
loopAnArrayOfArrays([ ['a', 'b', 'c'], ['d', 'e', 'f'] ]);
// console output:
  // a
  // b
  // c
  // d
  // e
  // f

loopAnArrayOfArrays([ [1, 2], [3, 4], [5], [6, 7, 8] ]);
// console output:
  // 1
  // 2
  // 3
  // 4
  // 5
  // 6
  // 7
  // 8
```

```javascript
function loopAnArrayOfArrays(arrayOfArrays) {
  // create a loop which iterates over the input array
    // create an inner loop which iterates over current inner array
      // log current element to the console
  for (var i = 0; i < arrayOfArrays.length; i++) {
    var innerArray = arrayOfArrays[i];
    for (var j = 0; j < innerArray.length; j++) {
        console.log(innerArray[j]);
    }
  }
}
```

#### For-in loop over an object of objects

We are going to complete a function that takes one parameter, a object of objects, and logs all of its values (log each value in first inner object, one at a time, then second inner object, and so on...) to the console. Your function should use a nested for-in loop to log each value from all inner objects, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopAnObjectOfObjects`.

```javascript
loopAnObjectOfObjects({ a: {a: 1, b: 2}, b: {a: 5, b: 6} });
// console output:
  // 1
  // 2
  // 5
  // 6

loopAnObjectOfObjects({ structures: {queue: true, stack: false}, plantLife: {tree: 'leaves'}, letters: {apple: 'a', bag: 'b', cats: 'c'} });
// console output:
  // true
  // false
  // leaves
  // a
  // b
  // c
```

```javascript
function loopAnObjectOfObjects(nestedObject) {
  // create a loop which iterates over the input object
    // create an inner loop which iterates over current inner object
      // log current value to the console
  for ( var key in nestedObject ) {
    for ( var innerKey in nestedObject[key]) {
        console.log(nestedObject[key][innerKey]);
    }
  }
}
```

#### Loop over an array of objects
Submitted on 10/12/2021
We are going to complete a function that takes one parameter, a array of objects, and logs all of its values (log each value in first inner object, one at a time, then second inner object, and so on...) to the console. Your function should use a `for-in` loop nested inside of a for loop to log each value from all inner objects, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopAnArrayOfObjects`.

```javascript
loopAnArrayOfObjects([{a: 1, b: 2}, {z: 5, y: 6}, {q: 14} ]);
// console output:
  // 1
  // 2
  // 5
  // 6
  // 14

loopAnArrayOfObjects([{queue: false, stack: true}, {fish: 'swims'}, {shirt: 's', pop: 'p', eye: 'e'} ]);
// console output:
  // false
  // true
  // swims
  // s
  // p
  // e
```

```javascript
function loopAnArrayOfObjects(arrayOfObjects) {
  // create a loop which iterates over the input array
    // create an inner loop which iterates over current inner object
      // log current value to the console
  for ( var i = 0; i < arrayOfObjects.length; i++) {
    var innerObj = arrayOfObjects[i];
    for ( var key in innerObj ) {
        console.log(innerObj[key]);
    }
  }
}
```

#### Loop over an object of arrays

We are going to complete a function that takes one parameter, a object of arrays, and logs all of its values (log each value in first inner array, one at a time, then second inner array, and so on...) to the console. Your function should use a for loop nested inside of a for-in loop to log each value from all inner arrays, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `loopAnObjectOfArrays`.

```javascript
loopAnObjectOfArrays({ first: [1, 2, 5], second: [6, 14, 21] });
// console output:
  // 1
  // 2
  // 5
  // 6
  // 14
  // 21

loopAnObjectOfArrays({ third: [false, false], fourth: ['runs'], ninth: ['q', 'l', 'z'] });
// console output:
  // false
  // false
  // runs
  // q
  // l
  // z
```

```javascript
function loopAnObjectOfArrays(objectOfArrays) {
  // create a loop which iterates over the input object
    // create an inner loop which iterates over current inner array
      // log current value to the console
  for (var key in objectOfArrays) {
    var innerArray = objectOfArrays[key];
    for (var i = 0;  i < innerArray.length ; i++) {
        console.log(innerArray[i]);
    }
  }
}
```

#### List all combinations of two arrays

We are going to complete a function that takes two parameters, both arrays, and logs all possible combinations of elements separated by a space (see example for details...) to the console. Your function should use a nested for loop to log all combinations of the two arrays, then return nothing. Below is an example of the code running, assuming that you will have completed the described function: `generateCombinations`.

```javascript
generateCombinations(['a', 'b', 'c'], ['d', 'e', 'f']);
// console output:
  // a d
  // a e
  // a f
  // b d
  // b e
  // b f
  // c d
  // c e
  // c f

generateCombinations([1, 2], ['buckle', 'my', 'shoe']);
// console output:
  // 1 buckle
  // 1 my
  // 1 shoe
  // 2 buckle
  // 2 my
  // 2 shoe
```

```javascript
function generateCombinations(array1, array2) {
  // create a loop which iterates over the first array
    // create an inner loop which iterates over the second array
      // log current element of first array and current element of second array to the console with space in between
  for ( var i = 0 ; i < array1.length ; i++) {
    for ( var j = 0 ; j < array2.length ; j++) {
        console.log(array1[i] + " " + array2[j]);
    }
  }
}
```

## Functions

### Accumulator Pattern

#### filterOddElements

Write a function called "filterOddElements".

Given an array of numbers, "filterOddElements" returns an array containing only the odd numbers of the given array. If the input array contains no odd numbered elements, your function should return an empty array.

```javascript
var output = filterOddElements([1, 2, 3, 4, 5]);
console.log(output); // --> [1, 3, 5]
```

```javascript
function filterOddElements(numbers) {
    if (numbers.length === 0) {
        return [];
    }
    var oddNumbers=[];
    for ( var i = 0 ; i < numbers.length; i++) {
        if (numbers[i] % 2 === 1) {
            oddNumbers.push(numbers[i]);
        }
    }
    return oddNumbers;
}
```

#### computeSumOfAllElements

Write a function called "computeSumOfAllElements".

Given an array of numbers, "computeSumOfAllElements" returns the sum of all the elements in the given array. If input array is empty, your function should return 0.

```javascript
var result1 = computeSumOfAllElements([1, 2, 3]);
console.log('should log 6:', result1);

var result2 = computeSumOfAllElements([]);
console.log('should log 0:', result2);
```

```javascript
function computeSumOfAllElements(numbers) {
    if (numbers.length === 0) {
        return 0;
    }
    var sum = 0;
    for (var i = 0; i < numbers.length; i++) {
        sum += numbers[i];
    }
    return sum;
}
```

#### Generate Average of Elements

Write a function called "computeAverageOfNumbers".

Given an array of numbers, "computeAverageOfNumbers" returns their average. If input array is empty, your function should return 0.

```javascript
var input1 = [1,2,3,4,5];
var result1 = computeAverageOfNumbers(input1);
console.log('should log 3:', result1);

var input2 = [];
var result2 = computeAverageOfNumbers(input2);
console.log('should log 0:', result2);
```

```javascript
function computeAverageOfNumbers(numbers) {
    if(numbers.length === 0) {
        return 0;
    }
    var sum = 0
    for (var i = 0; i < numbers.length; i++) {
    sum += numbers[i];
    }
    return sum / numbers.length;
}
```

### Scope Introduction

#### Find a value in an object Debugging

We are going to debug a function that takes in an object, and a target value. This function will iterate over the object's values, and attempt to locate the target value. If the value is found, the function should return the name of the key where the value in question is located, and if not, the function should return -1. Below is an example of the code running, assuming that you will have debugged the described function: `keyOfObjectValue`:

```javascript
var result1 = keyOfObjectValue({cucumbers: 14, carrots: 20, peas: 400}, 20);
console.log('should log "carrots":', result1);

var result2 = keyOfObjectValue({name: 'Bruce Wayne', hero: 'Batman', city: 'Gotham'}, 'Superman');
console.log('should log -1:', result2);
```

```javascript
function keyOfObjectValue(object, target) {
  for (var key in object) {
    if (object[key] === target) {
      return key;
    } 
  }
  return - 1;
}
```

#### Count Elements Above 40 Debugging

We are going to debug a function that takes in an array of numbers. This function will iterate over the array's number elements, and return a count representing the number of elements whose value is greater than 40. If there are no values above 40, then the function should return 0. Below is an example of the code running, assuming that you will have debugged the described function: `getElementsAbove40`:

```javascript
var result1 = getElementsAbove40([1, 42, 5, 314, 2, 89]);
console.log('should log 3:', result1);

var result2 = getElementsAbove40([1, 4, 3, 2, 6]);
console.log('should log 0:', result2);
````

```javascript
function getElementsAbove40(numbers) {
  var count = 0;
  for (var i = 0; i < numbers.length; i++) {
    if (numbers[i] > 40) {
      count++;
    }
  }
  return count;
}
```

#### Create a Sentence Debugging

We are going to debug a function that takes in an array of strings, representing words in a sentence. This function should iterate over the input array and should create, and return, a resulting sentence from the words therein. Below is an example of the code running, assuming that you will have debugged the described function: `createSentence`:

```javascript
var result1 = createSentence(['I', 'am', 'worth', 'it']);
console.log('should log "I am worth it.":', result1);

var result2 = createSentence(['My', 'problems', 'matter']);
console.log('should log "My problems matter.":', result2);
```

```javascript
function createSentence(words) {
  var sentence = "";
  for (var i = 0; i < words.length; i++) {
    // hint: does this line need to happen every iteration?
    if (i === words.length - 1){
        sentence += words[i] + '.';
    } else {
      sentence += words[i] + ' ';  
    }
  }
 return sentence;
}
```

### Data Modeling

#### Use an object to count words in a sentence

Write a function called "countWords".

Given a string (words separated by spaces), "countWords" returns an object where each key is a word in the given string, with its value being how many times that word appeared in the given string. If given an empty string, your function should return an empty object.

```javascript
var result1 = countWords('ask a bunch get a bunch');
console.log('should log "{ask: 1, a: 2, bunch: 2, get: 1}":', result1);

var result2 = countWords('');
console.log('should log "{}":', result2);
```

```javascript
function countWords(stringOfWords) {
 //if input is empty obj
 if ( stringOfWords === '' ) {
   // return empty obj
   return {};
}

  // create result count obj
  var counts = {};

  //split the inout string into an array of words
  var words = stringOfWords.split(' ');
    //iterate over the array of words
    for ( var i = 0; i < words.length; i++) {
      var currentWord = words[i];
      //check if current word is not in result obj
      if ( counts[currentWord] === undefined) {
    //instantiate current word in obj with value of 1
      counts[currentWord] = 1;
    //otherwise
    } else {
      // increment value of current word in obj by 1
      counts[currentWord]++;
    }
  }
// return the result count obj
return counts;
}
```

#### Use an object to count letters in a word

Write a function called "countAllCharacters".

Given a string of characters, "countAllCharacters" returns an object where each key is a character in the given string, with its value being how many times that character appeared in the given string. If given an empty string, your function should return an empty object.

```javascript
var result1 = countAllCharacters('banana');
console.log('should log "{b: 1, a: 3, n: 2}":', result1);

var result2 = countAllCharacters('');
console.log('should log "{}":', result2);
```

```javascript
function countAllCharacters(string) {
    if (string == '') {
        return {};
    }
    var counts = {};
    for ( var i = 0; i < string.length; i++) {
        if (counts[string[i]] === undefined ) {
            counts[string[i]] = 1;
        } else {
            counts[string[i]]++;
        }
    }
    return counts;
}
```

