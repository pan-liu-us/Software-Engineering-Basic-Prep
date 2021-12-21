## Testing

### assertEqual

### assertArraysEqual

### assertObjectsEqual

### assertWithinRange

### Sample of Clean Code Structure

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

### Applying assertEqual 1

### Applying assertEqual 2

### Applying assertArraysEqual

### Applying assertObjectsEqual


## Skeletons

### Average

### Decorate Student List

### Isograms

### Interpret A Skeleton

### Declaring Functions

### Render Phone Number (Optional)

### Find Longest Palindrome


## Fashion Inventory Problems

### Part A
### Part B
### Part C
### Part D
