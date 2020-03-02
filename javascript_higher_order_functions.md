# Higher Order Functions
### [Back to Concepts](./README.md)

## Syntax :
```JavaScript
// Map with Arrow Function
const array1 = [1, 4, 9, 16];
// pass a function to map
const map1 = array1.map(x => x * 2);
console.log(map1);
// expected output: Array [2, 8, 18, 32]
// Map without Arrow Function
let numbers = [1, 4, 9]
let roots = numbers.map(function(num) {
    return Math.sqrt(num)
})
// roots is now     [1, 2, 3]
// numbers is still [1, 4, 9]
// For Each 
const array1 = ['a', 'b', 'c'];
array1.forEach(element => console.log(element));
// expected output: "a"
// expected output: "b"
// expected output: "c"

const arraySparse = [1,3,,7]
let numCallbackRuns = 0
arraySparse.forEach((element) => {
  console.log(element)
  numCallbackRuns++
})
console.log(`numCallbackRuns: ${numCallbackRuns}`)
// 1
// 3
// 7
// numCallbackRuns: 3

// Filter
const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];
const result = words.filter(word => word.length > 6);
console.log(result);
// expected output: Array ["exuberant", "destruction", "present"]
```
## Definitions :
map calls a provided callback function once for each element in an array, in order, and constructs a new array from the results. callback is invoked only for indexes of the array which have assigned values (including undefined).

forEach() calls a provided callback function once for each element in an array in ascending order. It is not invoked for index properties that have been deleted or are uninitialized. The callback is invoked with three arguments:
the value of the element
the index of the element
the Array object being traversed

The filter() method creates a new array with all elements that pass the test implemented by the provided function.
## Reference Links :

[Eloquent JavaScript - High Order Functions](https://eloquentjavascript.net/05_higher_order.html)

[Dev.to - Higher Order Functions](https://dev.to/damcosset/higher-order-functions-in-javascript-4j8b)

[YouTube Video - Higher Order Functions](https://www.youtube.com/watch?v=rRgD1yVwIvE)

[Medium Article - Classes](https://medium.com/tech-tajawal/javascript-classes-under-the-hood-6b26d2667677)
