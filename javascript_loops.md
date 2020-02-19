# JavaScript Loops
#### [Back to Concepts](./README.md)

Often in our code we need to repeat a certain list of instructions multiple times. We might be passed an array of items, and for each item we want to do the same thing until we have processed the entire list of items.

We *could* just repeat the same code over and over enough times to process the items, and that works if we know ahead of time exactly how many items are in the list, but it's still not the best way to process the items. Why is it a bad idea? Well 1) Because you end up duplicating the same line(s) of code over, and over, and over... and 2) The number of items in the collection is rarely known ahead of time. Sometimes there may be 100 items to process while other times there's just a few.

Loops let us repeat the code in a code block as many times as needed a certain number of times and/or until a certain condition is met. Each pass through the code while looping is known as an *iteration*.

The most common types of loops across all languages are `for` loops and `while` loops. The type of loop you will choose depends on the type of processing going on. Sometimes we want to iterate through a loop a certain *number of times*. Other times we want to iterate through a loop until some *condition* is met like keep repeating until the user enters a certain command. In these cases, we may iterate through our loop 1 time, 20 times, or even 9001 times before the condition is met.

## For Loops
For loops are often the simpliest type of loop for new developers to understand. 
```js
for (begin; condition; step) {
  // ... loop body ...
}
```
While there are newer variations available today that are more sophisticated than the good old original for loop. In general, for loops are best used when we want to do something a certain number of times. Either we know ahead of time exactly how many times we want to iterate the loop e.g. give them `3` chances to correctly enter their password), or can infer this number from something else (e.g. like the `length` of the array we wish to process).
```js
for (let i = 0; i < 3; i++) { // shows 0, then 1, then 2
  alert(i);
}
```

## `while` Loops
Beginners tend to have more difficulty with `while` loops when first starting out.
```js
while (condition) {
  // code
  // so-called "loop body"
}
```
While loops are used when we want to keep doing something `while` some condition is true. For example. let the user keep entering names until they enter `quit` or keep prompting the user until they make a valid entry.
```js
let i = 0;
while (i < 3) { // shows 0, then 1, then 2
  alert( i );
  i++;
}
```

## `do…while` loop
The condition check can be moved below the loop body using the do..while syntax:
```js
do {
  // loop body
} while (condition);
```
The **most important** thing to not that is different about `do-while` loops, as the code block will *always* execute at least one time as the exit condition will not be checked until the end of the first iteration.
```js
let i = 0;
do {
  alert( i );
  i++;
} while (i < 3);
```
## Breaking out of Loops Early
Generally a loop will execute until whatever condition is met and then exit the loop and process the next line of code. However, you can prematurely terminate a loop using the `break` keyword.
```js
let sum = 0;

while (true) {

  let value = +prompt("Enter a number", '');

  if (!value) 
  {
      break; // (*)
  }

  sum += value;

}
alert( 'Sum: ' + sum );
```

## Continuing to the Next Iteration Early
During each iteation of a loop, we typically run each instruction inside the code block, returning to the top of the block when the end is reached to perform the next iteration.

However there will be times when you will want to proceed to the next iteration early skipping some of the remaining instructions in the loop. For example if while letting the user enter a name that is saved in a database, you will want to skip the database save part of the loop and go back to the top and prompt them again if the data they entered was invalid.

To skip the rest of the iteration and start back at the top of the code block for the next iteration, we can use the `continue` keyword.
```js
for (let i = 0; i < 10; i++) {

  // if true, skip the remaining part of the body
  if (i % 2 == 0) 
  {
      continue;
  }

  alert(i); // 1, then 3, 5, 7, 9
}
```

## Practice
- [For Loops](https://github.com/cs-fullstack-master/JavaScript-forLoops_ic)
- [While Loops 1](https://github.com/cs-fullstack-master/JavaScript-whileloops-ic)
- [While Loops 2](https://github.com/cs-fullstack-master/javaScript-week1-review)


## Additional Information
- [Adding Array Elements via Loops Video](https://youtu.be/n6pCS-w1M3o)
- [Eloquent JavaScript - Do Loops](https://eloquentjavascript.net/02_program_structure.html#p_FIHE6k56BA)
- [Eloquent JavaScript - For Loops](https://eloquentjavascript.net/02_program_structure.html#h_oupMC+5FKN)
- [MDN - Loops and Iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)


[BACK TO TOP](#JavaScript-Loops)
