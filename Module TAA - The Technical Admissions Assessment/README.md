## Advanced Pre-Assessment Practice

#### Altitude Deltas

Please write a function that takes an array of integer altitudes along a hiking trail, as well as two indexes into that array. The two indexes represent the start and end of a segment in the array. We can assume that the array will only contain integers, and that the two indexes will be valid (i.e. they will exist in the input array, and will make sense compared to each other - start is before end).

Your function should return the "sum of the changes for a walk within that segment" (i.e., beginning at the start index and ending at the end index). Each integer in the array represents another height on the trail, so "walking" will mean accumulating each change in height into a "sum of the changes".

Note that increases in height count double.

Here are some examples of your code running, assuming you have successfully created the described function. Please be sure to name the function "sumAltitudeDeltas".

```javescript
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

```javescript
// please complete the challenge according to the instructions

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

```javescript
let blackWinner = checkWinner(['black', 'red', 'black', 'black', 'black', 'black', 'red']);
console.log(blackWinner); //-> 'Black Wins!'

let redWinner = checkWinner([0,0,0, 'red', 'red', 'red', 'red']);
console.log(redWinner); //-> 'Red Wins!'

let draw = checkWinner(['red', 'red', 'red', 'black', 'red', 'black', 0]);
console.log(draw); // -> 'Draw!'
```

```javescript
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
