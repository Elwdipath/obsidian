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
  - algorithm
  - bigo
  - spacialcomplexity
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


```javascript
function getMiddleOfArray(array) {
  return array[Math.floor(array.length / 2)];
}
```

This would be O(1) because no matter how long the array is, this still takes the same amount of time to do.

![[Software Development Courses/attachments/BigOgraph.png]]
Red = O(1) Example: getMiddleOfArray() function will take the same amount of time to run no matter the size of the array. 

Blue = The blue line represents a function that takes longer based on how many items are in the array similar to `crossAdd` or `find` and it grows a steady rate. If it takes 10ms to run a function with a 100 items in it, we could reasonably expect it would take 10 times longer-ish (remember, these are broad strokes, not precise figures) if we had 10 times the amount of things in the array.

Green = The green line is where we get start getting scary. For every item we add to the array, it takes exponentially more time to complete the operation. Adding 10x the items could cause a function to takes 100x longer since it's O(n²). It gets even scarier at O(n³) as it would take 1000x longer.


![[Software Development Courses/attachments/BigOgraph-log.png]]
Notice the purple line we added. Now as we add more terms to the array, it takes less and less time because the function can make some use of some tricks to take shortcuts. We'll dig into these later in the course.
### Links
https://btholt.github.io/complete-intro-to-computer-science/big-o/

## Spacial Complexity

### Linear

Let's say we have an algorithm that for every item in the array, it needs to create another array in the process of sorting it. So for an array of length 10, our algorithm will create 10 arrays. For an array of 100, it'd create 100 extra arrays (or something close, remember these are broad strokes, not exact.) This would be O(n) in terms of its spatial complexity. We'll do some sorts that do this.
### Logrithmic
What about another for every item in the array, it needed to create a diminishing amount of extra arrays. For example: for an array of length 10, it'd create 7 arrays. For an array of 100, it'd create 12 arrays. For an array of 1000, it'd created 20 arrays. This would be O(log n).
### Constant
What if we didn't create any extra arrays when we did our algorithm? We just used the same space we were given when we first started. Or if we created just 10 arrays, no matter how long the array is? This would be O(1) since it's constant no matter what. Its spatial need don't increase with longer arrays.

### Quadratic

Lastly, what if we had an app that calculates the distances between zip / postal codes?

> A zip code in the United States is a five digit number that represents a fairly small area of land. 98109 is in the middle of Seattle, Washington while 10001 is in the middle of New York City, NY.

If a user asks what's the distance between 98109 and 10001, we'd spit out something like 2,800 miles or 4,500 km. Now, let's say for every zip code we add to our system, we calculate the distance between every other zip code in our system and store it. If there were only 10 zip codes, sure, that'd be easy, but there are nearly 42,000 zip codes in the United States with more being added. The spatial complexity on this would be O(n²) because for every new zip code we add, we'd have to add 42,000 new items as well.

Is this a good idea? It depends! A company I used to work at did exactly this because calling the API to get this data was really expensive so they did all the computational work once to find out and just stored it. It was a huge database but that ended up being way cheaper than the API.

I will say O(n²) in spatial complexity is pretty rare and a big red flag.
### Links
https://btholt.github.io/complete-intro-to-computer-science/spatial-complexity/