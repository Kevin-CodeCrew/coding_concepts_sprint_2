# PreWork 
##### [Back to Concepts](./README.md)

#### CodePen Tutorial 
https://codepen.io/hello/

### Comments
Comments are used through the assignment to either give directions or clarify what a line of code does or represents. Typically in web development comments are used to let other developers (or your future self) know how/why something works. Commenting your code (and reading others comments) is an important skill for junior developers. Comments look different in different languages. Anytime you see a comment in a file remember that it will not execute (or have any affect on the code), it's just a note to the developer. 
```HTML
<!-- this is a comment in HTML and it will not display on the page -->
```
```CSS
/* this is a comment in CSS and it will not affect styling */
```
```JavaScript
// this is a comment in JS and it will not execute
```

### HTML
HTML is not a programming language; it is a markup language that defines the structure of your content. HTML consists of a series of [elements](https://developer.mozilla.org/en-US/docs/Glossary/element), which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way. The enclosing [tags](https://developer.mozilla.org/en-US/docs/Glossary/tag) can make a word or image hyperlink to somewhere else, can italicize words, can make the font bigger or smaller, and so on
#### Syntax

<img src="./img/htmlSyntax.png" alt="html syntax example" width="300"/>

1. The opening tag: This consists of the name of the element (in this case, p), wrapped in opening and closing angle brackets. This states where the element begins or starts to take effect — in this case where the paragraph begins.
2. The closing tag: This is the same as the opening tag, except that it includes a forward slash before the element name. This states where the element ends — in this case where the paragraph ends. Failing to add a closing tag is one of the standard beginner errors and can lead to strange results.
3. The content: This is the content of the element, which in this case, is just text.
4. The element: The opening tag, the closing tag and the content together comprise the element.

There are several different HTML elements but primary ones you will be using for the pre-work challenge are [headings](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics#Headings) and [paragraphs](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics#Paragraphs).Heading elements and paragraph element are used to establish hierarchy. Heading tags allow you to style content in a set font size and weight and paragraph tags allow you to style content with a default top and bottom margin (or space above and below the content)

So this code snippet...
```HTML
<!-- title of the page at the largest heading -->
<h1>Page Title</h1>
<!-- subtitle of the page at a smaller heading -->
<h3>Page Subtitle</h3>
<!-- filler text paragraph element -->
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</p>
```
...displays like this on the page
<hr>
<h1>Page Title</h1>
<h3>Page Subtitle</h3>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.</p>
<hr>

#### Grouping Elements
In addition to defining individual parts of your page (such as "a paragraph"), HTML also boasts a number of [block level elements](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started#Block_versus_inline_elements) used to define areas of your website (such as "the header" or "the main content"). Sometimes you'll come across a situation where you can't find an ideal semantic element to group some items together or wrap some content. Sometimes you might want to just group a set of elements together to affect them all as a single entity with some CSS or JavaScript. For cases like these, HTML provides the `<div>` and `<span>` elements. You should use these preferably with a suitable class attribute, to provide some kind of label for them so they can be easily targeted. You'll notice the `<div>` tag is used in the pre-work challenge primarily to provide styling to nested `<p>` elements. We will look more into styling in the CSS section below. 
#### Attributes
<img src="./img/attributes.png" alt="html syntax example" width="300"/>

Attributes contain extra information about the element that you don't want to appear in the actual content. In this case, the class attribute allows you to give the element an identifying name, that can be used later to target the element with style information and other things.

An attribute should have:

- A space between it and the element name (or the previous attribute, if the element already has one or more attributes).
- The attribute name, followed by an equal sign.
- An attribute value, with opening and closing quote marks wrapped around it.

[Class](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Type_Class_and_ID_Selectors#Class_selectors) attributes are used to applying styling to multiple elements by name while [id](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors/Type_Class_and_ID_Selectors#ID_Selectors) attributes are used to applying styling to one element by name. We will look more into styling in the CSS section below.

[Event Listeners](https://developer.mozilla.org/en-US/docs/Web/Guide/Events/Event_handlers#HTML_onevent_attributes)

### CSS
#### Selectors
#### Font Color
#### Background Color
#### Margin and Padding

### JavaScript
#### Functions
#### Event Handlers
#### Alert
#### Console Log
#### getDocumentById
#### Inner Text

##### [BACK TO TOP](#PreWork)
