---
type: course
title: Algorithm Analysis
provider: Frontend Masters
status: In Progress
start_date: ""
finish_date: ""
tags:
  - course
  - learning
  - introcs
platform:
---
#course #introcs 

 
## Big O

Big is a way of talking about how efficient an algorithm is (mathematically)

A "term" in mathematics just means one piece of the equation (normally separated by + or - signs). In 3x² + x + 1, 3x² is the first term, x is the second, and 1 is the third.

Example: An array with a length of 1 would be (3(1)^2) + 1 + 1 = 5
Big O can be simplified to use $O(n^2)$ since we're more interested in the biggest "terms" of the equation

```javascript
function crossAdd(input) {
  var answer = [];
  for (var i = 0; i < input.length; i++) {
    var goingUp = input[i];
    var goingDown = input[input.length - 1 - i];
    answer.push(goingUp + goingDown);
  }
  return answer;
}
```


How many instructions am I giving the CPU based on the length of the array?

Anything outside the loop will only execute once while code inside the loop will execute for each iteration of the loop. input.length can be calculated using $O(n)$

```javascript
function find(needle, haystack) {
  for (var i = 0; i < haystack.length; i++) {
    if (haystack[i] === needle) return true;
  }
}
```

Still $O(n)$


```javascript
function makeTuples(input) {
  var answer = [];
  for (var i = 0; i < input.length; i++) {
    for (var j = 0; j < input.length; j++) {
      answer.push([input[i], input[j]]);
    }
  }
  return answer;
}
```
This would be O(n²). For every input, we have to go through a full loop inside of another full loop, meaning we're doing a lot of work! This is the trick: look for loops. A loop inside of a loop inside of a loop would likewise be O(n³).

If we have no loops and just do something and exit/return, then it's said we're doing it in constant time, or O(1).




## Links
https://btholt.github.io/complete-intro-to-computer-science/big-o/