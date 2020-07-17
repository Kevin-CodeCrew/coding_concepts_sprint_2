# Conditionals

### Resources 
- [MDN Overview](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)
- [JS Info Comparisons](https://javascript.info/comparison)
- [JS Info If Statements](https://javascript.info/ifelse)
- [JS Info Logical Operators](https://javascript.info/logical-operators)
### Extra Practice
- [200716-js-conditionals-extra-1](https://classroom.github.com/a/jXbP88lA)

### SYNTAX
```JS
if (`some condition`) {
    `code to run if condition is true`;
}

if (`some condition`) {
    `code to run if condition is true`
} else {
    `code to run if condition is false`
}

if (`some condition`) {
    `code to run if condition is true`
} else if (`some other condition`) {
    `code to run if other condition is true`
} else {
    `code to run if above conditions are false`
}
```
### BASIC IF STATEMENT
```JS
let testName = "Autumn"; // define a variable

if (testName == "Autumn") { // if value of variable testName is "Autumn"
    // print message
    console.log("The test name is Autumn");
}
```
### COMPARISONS
- `==` : are values equal
- `===` : are values and type equal
- `!=` : are values not equal
- `>` : greater than
- `<` : less than 
### EXTRA
- `% 2` : remainder after division by 2
#### Examples of equality between strings
```JS
let nameOne = "Kenn";
let nameTwo = "Kevin";
// this condition evaluates to false
if (nameOne == nameTwo) { // if the value of variable nameOne and nameTwo are equal
    // print message
    console.log("The names are the same!");
}
// this condition evaluates to true
if (nameOne != nameTwo) { // if the value of variable nameOne and nameTwo are not equal
    // print message
    console.log("The names are not the same");
}
```
#### Examples of equality between strings and integers
```JS
let userNum = prompt("Enter the number 35"); // get user input
let userNumInt = parseInt(userNum); // define variable with userNum as integer
let intAge = 35; // define variable with integer 35

// this condition evaluates to false
if (intAge === userNum) { // if the value of variable userNum and intAge are equal and the same value
    // print message
    console.log("Int Age and User Num are strictly equal");
}
// this condition evaluates to true
if (intAge === userNumInt) { // if the value of variable userNum and intAge are equal and the same value
    // print message
    console.log("Int Age and User Num Int are strictly equal");
}
```
#### Examples of math comparisons between integers
``` JS
let num1 = 50; // define a variable
let num2 = 25; // define a variable

// this condition evaluates to false
if (num1 < num2) { // if the value of variable num1 is greater than the value of variable num2
    // print message
    console.log("Number one is less than Number 2");
}

// this condition evaluates to true
if (num1 > num2) { // if the value of variable num1 is less than the value of variable num2
    // print message
    console.log("Number one is greater than Number 2");
}

// this condition evaluates to false
if (num1 == num2) { // if the value of variable num1 is equal to the value of variable num2
    // print message
    console.log("Number One is equal to Number Two");
}
```
### IF ... ELSE STATEMENT
#### Examples of if .. else
```JS
num1 = 50; // define a variable
num2 = 25; // define a variable

if (num1 < num2) { // if the value of variable num1 is greater than the value of variable num2
    // print message
    console.log("Number One is less than number two");
} else { // OTHERWISE if the value of variable num1 is NOT greater than the value of variable num2
    // print message
    console.log("Number One is greater than number two");
}
```
#### Examples of else if
```JS
if (num1 < num2) { // if the value of variable num1 is less than the value of variable num2
    // print message
    console.log("Number One is less than number two");
} else if (num1 > num2) { // OTHERWISE if the value of variable num1 is greater than the value of variable num2
    // print message
    console.log("Number One is greater than Number 2");
} else { // OTHERWISE if the value of variable num1 is NOT greater than OR less than the value of variable num2
    // print message
    console.log("Number One and Number Two are equal");
}
```
### NESTED IF STATEMENT 
#### Examples of and if statement in an if statement
```JS
num1 = 55; // define a variable

if (num1 > num2) { // if the value of variable num1 is greater than the value of variable num2
    // nested if that only runs if the above if statement evaluates to true
    if (num1 % 2 == 0) { // if the value of variable num1 has no remainder when divided by 2
        // print message
        console.log("Number 1 is the greater Number AND divisible by 2");
    } else { // OTHERWISE if the value of variable num1 DOES have a remainder when divided by 2
        // print message
        console.log("Number 1 is greater than Number 2");
    }
} else { // if the value of variable num1 is NOT greater than the value of variable num2
    // print message
    console.log("Number 1 is not greater than Number 2");
}
```
### LOGICAL OPERATORS
- `AND` : && -- TRUE `AND` TRUE = TRUE; TRUE `AND` FALSE = FALSE; FALSE `AND` FALSE = FALSE
- `OR` : || -- TRUE `OR` TRUE = TRUE; TRUE `OR` FALSE = TRUE; FALSE `OR` FALSE = FALSE

#### Examples of OR operator
```JS
let codeCrewTeamOne = "Autumn"; // declare variable
let codeCrewTeamTwo = "Kevin"; // declare variable
let codeCrewTeamThree = "Kenn"; // declare variable

// this condition evaluates to true
if (codeCrewTeamTwo == "Erin" || codeCrewTeamThree == "Kenn") { // if the value of the variable codeCrewTeamTwo  is "Erin" OR the value of the variable codeCrewTeamThree is "Kenn"
    // print message
    console.log("At least one is a team member");
} else { // OTHERWISE if the value of the variable codeCrewTeamTwo  is not "Erin" AND the value of the variable codeCrewTeamThree is not "Kenn"
    // print message
    console.log("At least one is a team member");
}

// this condition evaluates to false
if (codeCrewTeamTwo == "Erin" || codeCrewTeamThree == "Meka") { // if the value of the variable codeCrewTeamTwo  is "Erin" OR the value of the variable codeCrewTeamThree is "Meka"
    // print message
    console.log("At least one is a team member");
} else { // OTHERWISE if the value of the variable codeCrewTeamTwo  is not "Erin" AND the value of the variable codeCrewTeamThree is not "Meka"
    // print message
    console.log("At least one is a team member");
}
```
#### Examples of AND operator
```JS
let codeCrewTeamOne = "Autumn"; // declare variable
let codeCrewTeamTwo = "Kevin"; // declare variable
let codeCrewTeamThree = "Kenn"; // declare variable

// this condition evaluates to true
if (codeCrewTeamTwo == "Kevin" && codeCrewTeamThree == "Kenn") {// if the value of the variable codeCrewTeamTwo  is "Kevin" AND the value of the variable codeCrewTeamThree  is "Kenn"
    // print message
    console.log("Both are team members");
} else { // OTHERWISE if the value of the variable codeCrewTeamTwo  is not "Kevin" AND the value of the variable codeCrewTeamThree  is "Kenn"
    // print message
    console.log("At least one is a team member");
}
// this condition evaluates to 
if (codeCrewTeamTwo == "Meka" && codeCrewTeamThree == "Erin") {// if the value of the variable codeCrewTeamTwo  is "Erin" AND the value of the variable codeCrewTeamThree  is "Meka"
    // print message
    console.log("Both are team members");
} else { // OTHERWISE if the value of the variable codeCrewTeamTwo  is not "Erin" OR the value of the variable codeCrewTeamThree is not "Meka" 
    // print message
    console.log("At least one is a team member");
}
```
