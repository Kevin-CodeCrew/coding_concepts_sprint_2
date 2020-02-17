# JavaScript - Formatting Text Output with Templates

Template literals (originally called `Template strings`), were introduced in ES6 to make it much easier for developers to produce formatted text output. Prior to `Template Literals`, when your program needed to print out some text consisting of both static text and variable data, you would usually *concatenate* the different data together into a big `string` using the `+` operator as in:

```
// Declare 2 variables to hold the 2 scores
let homeTeamScore = 87;
let visitingTeamScore = 72;

// Build a string to print usic fixed/static text and score variables
let finalScoreString = 'The final score was:' + '\n' + 
 ' Vistors - ' + visitingTeamScore + '\n' + ' The Home Team - ' + homeTeamScore + '\n';

// Print out the concatenated string
console.log(finalScoreString);
```
Expected Output:
```
The final score was:
 Vistors - 72
 The Home Team - 87
 ```
Building and output string using the `+` operator can get messy fast, and because you have to keep up of where you need to add an extra space betweens and/or line breaks (`\n`) makes it easy to make mistakes and end up with poorly formatted output on the screen or in your error logs. Template literals address many of these frustrating concerns and allows you to specify a template that is much more heman readable and less error prone. 

In JavaScript, template literals are simply strings that use special characters/patterns to designate where variable data should but output. Unlike standard strings in JavaScript that use single (`'`) or double (`"`) quotes, a template string is enclosed by the backtick (`` ` ``)  (grave accent) character.

Template literals can contain placeholders for variable data or any valid JavaScript expression. These are indicated by the dollar sign and curly braces `${expression}`. The expressions in the placeholders and the text between the backticks (`` ` ``) get passed to a function that will process it and returned a formatted string. The formatted string can be used just as any other string value and can be printed or stored in a variable or file for use later.


Let's refactor the code above to use template literals instead of string concatenation.
> Take special note of how we build the output string in the variable `finalScoreString`. 

```
// Declare 2 variables to hold the 2 scores
let homeTeamScore = 87;
let visitingTeamScore = 72;

// Build a string to print usic fixed/static text and score variables
let finalScoreString = 
`The final score was:
  Vistors - ${visitingTeamScore}
  The Home Team - ${homeTeamScore}
`;

// Print out the concatenated string
console.log(finalScoreString);
```
With template literals, you type a template string that more natually resembles the disered output, with natual spacing around values, including line breaks were desired.Note how in this example, the name in `${the_expression}` matches the variable name(s) that return the value in the variable when we output it in the console.

> For now, it is OK to assume that your placeholders will match the names of variables in your code, but get used to hearing the term `expression` as it comes up frequently in JavaScript and other programming languages. It simply means passing items that can be evaluated/executed by the JavaScript runtime. For example a simple variable expression, just returns the current value of the variable when evaluated
## Practice:
[Template Strings Practice 1](https://github.com/cs-fullstack-master/javascript-template-strings-ic2)
