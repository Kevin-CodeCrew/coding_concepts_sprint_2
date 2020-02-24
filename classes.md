# Classes
### [Back to Concepts](./README.md)

## Basics :
```JavaScript
// Class Definition
class Rectangle {
  constructor(height, width) { // initialize instance of class
    this.height = height;
    this.width = width;
  }
  // Method
  calcArea() {
    return this.height * this.width; // return height of object times width of object
  }
}
// New Insatnce of Class
let square = new Rectangle(10, 10);
console.log(square.calcArea()); // call a class method on an instance of that class (returns 100)
```
## Definitions :
- Class : A class is a type of function, but instead of using the keyword function to initiate it, we use the keyword class, and the properties are assigned inside a constructor() method
- Constrctor : The constructor method is special, it is where you initialize properties, it is called automatically when a class is initiated, and it has to have the exact name "constructor".
- Object : An instance of a class.
- Method : A method is a function for an instance of a class. You call the method by referring to the object's method name followed by parentheses (any parameters would go inside the parentheses).

## Refrence Links :

[MDN - Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

[JavaScript Info - Classes](https://javascript.info/class)

[Eloquent JavaScript - Classes](https://eloquentjavascript.net/06_object.html)

[Medium Article - Classes](https://medium.com/tech-tajawal/javascript-classes-under-the-hood-6b26d2667677)


## Lecture Gist :

[https://gist.github.com/autumn-ragland/1ef2ac1073c1f616fb60e1b8f1d64666#file-classes_lecture-js](https://gist.github.com/autumn-ragland/1ef2ac1073c1f616fb60e1b8f1d64666#file-classes_lecture-js)

## Extra Practice :

[]()

## IC Assignment Link : 

[]()

## IC Answers :

[https://gist.github.com/autumn-ragland/1ef2ac1073c1f616fb60e1b8f1d64666#file-classes_ic-js](https://gist.github.com/autumn-ragland/1ef2ac1073c1f616fb60e1b8f1d64666#file-classes_ic-js)

## CW Assignment Link :

[]()

## CW Answers :

[https://gist.github.com/autumn-ragland/1ef2ac1073c1f616fb60e1b8f1d64666#file-classes_cw-js](https://gist.github.com/autumn-ragland/1ef2ac1073c1f616fb60e1b8f1d64666#file-classes_cw-js)

## Classwork Review Video :

[]()

### [BACK TO TOP](#Classes)