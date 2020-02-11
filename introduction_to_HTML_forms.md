# Introduction to HTML Forms
#### [Back to Concepts](./README.md)
-------------------
Forms allow us to get data input from Users to feed to our web applications. Users can fille out our form and submit the data to the server for processing.

### Form Element
The HTML <form> element defines a form that is used to collect user input:

```
<form>
.
  form elements
.
</form>
```

### The `<input>` Element
The `<input>` element is the most important form element. Users enter data via `input` elements.

The `<input>` element can be displayed in several ways, depending on the type attribute. The `type` attribute also can be used
 perform some action, validation and/or formatting for you depending on the type. For example, type `password` input element will hide the characters that the User types in.

Here are some examples:

`<input type="text">`	Defines a one-line text input field
`<input type="radio">`	Defines a radio button (for selecting one of many choices)
`<input type="submit">`	Defines a submit button (for submitting the form and the data entered into it)

You will learn a lot more about input types later in this class.



### HTML Input Types
There are the many different input types you can use in HTML:

```
<input type="button">
<input type="checkbox">
<input type="color">
<input type="date">
<input type="datetime-local">
<input type="email">
<input type="file">
<input type="hidden">
<input type="image">
<input type="month">
<input type="number">
<input type="password">
<input type="radio">
<input type="range">
<input type="reset">
<input type="search">
<input type="submit">
<input type="tel">
<input type="text">
<input type="time">
<input type="url">
<input type="week">
```

#### Example
```
<form>
  User name:<br/>
  <input type="text" name="username"><br>
  User password:<br/>
  <input type="password" name="psw">
</form>
```

---------------
[BACK TO TOP](#introduction-to-html-forms)