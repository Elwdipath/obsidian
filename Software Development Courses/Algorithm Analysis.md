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

Anything outside the loop will only execute once while code inside the loop will execute for each iteration of the loop. input.length can be calculated using n^2

```javascript
function find(needle, haystack) {
  for (var i = 0; i < haystack.length; i++) {
    if (haystack[i] === needle) return true;
  }
}
```

Still $n^2$
## Links
https://btholt.github.io/complete-intro-to-computer-science/big-o/