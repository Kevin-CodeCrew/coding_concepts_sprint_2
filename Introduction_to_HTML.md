# Introduction to HTML
HTML (**H**yper**t**ext **M**arkup **L**anguage) is the code that is used to structure a web page and its content. For example, content could be structured within a set of paragraphs, a list of bulleted points, or using images and data tables. As the title suggests, this article will give you a basic understanding of HTML and its functions.

## HTML Concepts
HTML is not a programming language; it is a markup language that defines the structure of your content. HTML consists of a series of elements, which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way. The enclosing tags can make a word or image hyperlink to somewhere else, can italicize words, can make the font bigger or smaller, and so on.  For example, take the following line of content:

`My cat is kind of a punk`

If we wanted the line to stand by itself, we could specify that it is a paragraph by enclosing it in paragraph tags:

`<p>My cat is kind of a punk</p>`

As far as it's relationship to the other key technologies such as [CSS](https://en.wikipedia.org/wiki/Cascading_Style_Sheets) and [JavaScript](https://en.wikipedia.org/wiki/JavaScript), [HTML](https://en.wikipedia.org/wiki/HTML), it is often described as 1 of 3 in *the triad* of core web development technologies (HTML, CSS, JavaScript).

It is often useful to think about the 3 complimenting technologies as a noun-adjective-verb relationship.

* The **Noun** HTML - HTML is the what, such as a paragraph
* The **Adjective** CSS - CSS defines the characteristics about the HTML content such as is **bold**
* The **Verb** JavaScript - JavaScript defines actions about the HTML such as 'hide this paragraph' or 'show' the form when the user clicks a button

### Elements

![Coolest Geek Tatoo Ever](./img/head_body.jpg)

Generally in HTML, we markup content with tags that include a starting tag and an ending tag. All tags are in less/greater than signs/characters. The opening tag does not contain a slash while the ending tag does. That's how the browser knows where the markup starts and ends. Take for instance, the following paragraph. 

`<p>This is a song about nothing. This is a song about nothing at all. #POWERMAN5000</p>`

> NOTE the start and end of the markup.

The idea is that we **markup** the data to display. The browser will apply default formatting, but as a developer we have *complete control* and thus can override any default display characteristics.

The start/and stop elements just tell the browser where to start and end the formatting.

#### Self Closing Elements
There are a handful of elements that **only** have a start tag and no formal end tag. This is a legacy issue in that early versions of HTML really wasn't thinking that we would every programmatically retrieve and parse random web content (think Google) thus the [creators of HTML](https://en.wikipedia.org/wiki/Tim_Berners-Lee) really didn't consider how the data would be constructed such that it was easy to process. 

When [XML](https://en.wikipedia.org/wiki/XML) appeared, and consequently [XHTML](https://en.wikipedia.org/wiki/XHTML), it enforced much stronger rules about matching tags in markup content in that **every** tag should have a closing tag or a self-closing tag if a traditional single tag markup element.

Example of valid but not best practice single HTML element

`<img src='./img/bugs.png>`

then a proper self-closing tab (note slash before end bracket)

`<img src='./img/bugs.png/>`

### Attributes
Attributes are optional values you can specify with an HTML element. Depending on the element, some are required, but most are used to tweak how the element is handled. Setting image width and/or height a good example.

Attributes are always specified in the **beginging** tag and not as part of the element content or closing tag.

`<img src='./img/bugs.png height='300' width='100' alt='Bugs Bunny'/>`

### HTML Document Structure
The main structure of HTML documents hasn't changed drastically over the years, but with the introduction of HTML5 semantic elements were introduced. 

Let's start with the primary sections of `<html>`, `<head>`, and `<body>` as well as directives.

#### Declarations
In the development world, **declarations** are extra information that is provided so that processing entities can better predict the type of data they are dealing with. This includes programs like web browsers.

Every HTML document should start with a declaration that specifies which version of HTML it conforms to as well as any additional [metadata](https://en.wikipedia.org/wiki/Metadata) that assists in processing of the document. While technically they are not required, it is a best practice to use them.

As of HTML5 you can get by with a simple declaration if your HTMl is up to spec.

`<!DOCTYPE html>`

#### HEAD
The `head` portion of an HTML document is loaded first and contains items that will not be displayed within the browser window. There are many elements that only can appear in the `head` portion such as `<title>` which is used to specify the text that will show at the top of the window/tab when the page is displayed.

An example of an element that may or may not be in the HEAD section is the `<script>` tag used for specifying JavaScript. The `<script>` tag can appear anywhere in your HTML. If your JavaScript is not manipulating elements in the [DOM](https://en.wikipedia.org/wiki/Document_Object_Model) then you should specify/include it in the HEAD portion of your HTML. However if your JavaScript depends on specific elements in the DOM, make sure your JavaScript is specified/included **after** the markup for the elements that it interacts with. This is because until those elements are rendered, they are not accessible. The DOM will be covered in more detail in subsequent modules.

#### BODY
Any content that you want rendered in the browser should appear in the BODY section of your HTML. Any valid HTML element can appear in this section, however only content that generates output that can be *rendered* in the browser will be displayed.

# Practice
* [Basics 1](https://github.com/cs-fullstack-master/html-basics1-ic)

* [Basics 2](https://github.com/cs-fullstack-master/html-basics1-cw)

# Additional Information
1. [Building Your First Web Page](https://learn.shayhowe.com/html-css/building-your-first-web-page/)
