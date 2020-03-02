# Selectors 
### [Back to Concepts](./README.md)

## Syntax :
```JavaScript
// Query Selector
let firstPTag = document.querySelector("p"); // get element by tag name
let firstPTagByID = document.querySelector("#first"); // get element by ID
let firstPTagByClass = document.querySelector(".special"); // get element by class name

// Query Selector All
let specialClassElements = document.querySelectorAll(".special"); // get ALL elements with class name
specialClassElements.forEach(el => console.log(`Special Class Query All Selected: ${el.innerText}`)); // iterate through array of elements
```
The short example above, like nearly all of the examples in this reference, is JavaScript. That is to say, it's written in JavaScript, but it uses the DOM to access the document and its elements. The DOM is not a programming language, but without it, the JavaScript language wouldn't have any model or notion of web pages, HTML documents, XML documents, and their component parts (e.g. elements). Every element in a document—the document as a whole, the head, tables within the document, table headers, text within the table cells—is part of the document object model for that document, so they can all be accessed and manipulated using the DOM and a scripting language like JavaScript.

In the beginning, JavaScript and the DOM were tightly intertwined, but eventually, they evolved into separate entities. The page content is stored in the DOM and may be accessed and manipulated via JavaScript, so that we may write this approximative equation:

API = DOM + JavaScript

The DOM was designed to be independent of any particular programming language, making the structural representation of the document available from a single, consistent API.
## Common APIs in Web Scripting using the DOM :

```
document.getElementById(id)
document.getElementsByTagName(name)
document.createElement(name)
parentNode.appendChild(node)
element.innerHTML
element.style.left
element.setAttribute()
element.getAttribute()
element.addEventListener()
window.content
window.onload
window.scrollTo()
```

## Refrence Links :

[https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

[https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementsByName](https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementsByName)

[https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementById](https://developer.mozilla.org/en-US/docs/Web/API/Document/getElementById)

## Classwork Link : 
https://classroom.github.com/a/qGGXKOpk

## Classwork Answers : 
https://gist.github.com/autumn-ragland/b78d34ca6c4f42d40a7e049eb5f8640d#file-cw-js

## Classwork Review Video :
[https://youtu.be/aEcjza7Jt3Q](https://youtu.be/aEcjza7Jt3Q)
 
### [BACK TO TOP](#Selectors)