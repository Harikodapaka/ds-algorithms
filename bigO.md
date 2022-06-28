# Big Os
O(1), O(logN), O(n), O(n Log(n)), O(n^2), O(2^n), O(n!)

# Time Complexity

## What Can Cause Time in a Function:
- Operations
- Comparisons
- Looping
- Outside Function call

Two separate collections: O(a * b)

**O(1) Constant** - no loops

**O(log N) Logarithmic** - usually searching algorithms have log n if they are sorted (Binary Search)

**O(n) Linear** - for loops, while loops through n items

**O(n log(n)) Log Linear** - usually sorting operations

**O(n^2) Quadratic** - every element in a collection needs to be compared to ever other element. Two nested loops

**O(2^n) Exponential** - recursive algorithms that solves a problem of size N

**O(n!) Factorial** - you are adding a loop for every element

Iterating through half a collection is still O(n)

Examples of O(n):
```
function anotherFunChallenge(input) {
  let a = 5;
  for (let i = 0; i < input; i++) {
    let x = i + 1;
  }
  for (let j = 0; j < input; j++) {
    let q = j * 2;
  }
}
```
Examples of O(n^2):
```
function anotherFunChallenge(input) {
  for (let i = 0; i < input; i++) {
    for (let j = 0; j < input; j++) {
        let q = j * i;
    }
  }
}
```
Examples of O(n+m):
```
function anotherFunChallenge(input1, input2) {
  // two different loop
  for (let i = 0; i < input1; i++) {
    let x = i + 1;
  }
  for (let j = 0; j < input2; j++) {
    let q = j * 2;
  }
}
```
Examples of O(n*m):
```
function anotherFunChallenge(input1, input2) {
  // two different loop
  for (let i = 0; i < input1; i++) {
    let x = i + 1;
    for (let j = 0; j < input2; j++) {
        let q = j * 2;
    }
  }
}
```

# Space Complexity
## What Causes Space Complexity:
- Variables
- Data Structures
- Function Call
- Allocations

### Space complexity O(1)
```
function boooo(n) {
    for (let i = 0; i < n; i++) {
        console.log('booooo');
    }
}
```
### Space complexity O(n)
```
function arrayOfHiNTimes(n) {
    var hiArray = [];
    for (let i = 0; i < n; i++) {
        hiArray[i] = 'hi';
    }
    return hiArray;
}
```