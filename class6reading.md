Read: 06 - Dynamic web pages with JavaScript

There are 3 ways to declare a JavaScript variable:

Using var
Using let
Using const

Variables
Variables are containers for storing data (values).

In this example, x, y, and z, are variables, declared with the var keyword:

Example
var x = 5;
var y = 6;
var z = x + y;


All JavaScript variables must be identified with unique names.

These unique names are called identifiers.

You can also add strings, but strings will be concatenated:
Example
var x = "John" + " " + "Doe"; output JohnDoe

Reserved words (like JavaScript keywords) cannot be used as names

It's a good programming practice to declare all variables at the beginning of a script.

Start the statement with var and separate the variables by comma:
var person = "John Doe", carName = "Volvo", price = 200;

A variable declared without a value will have the value undefined.
e.g var carName;

As with algebra, you can do arithmetic with JavaScript variables, using operators like = and +:
Example
var x = 5 + 2 + 3; output 10

If you put a number in quotes, the rest of the numbers will be treated as strings, and concatenated.

Since JavaScript treats a dollar sign as a letter, identifiers containing $ are valid variable names:
Example
var $$$ = "Hello World";
var $ = 2;
var $myMoney = 5; output 7

In the JavaScript library jQuery, for instance, the main function $ is used to select HTML elements. In jQuery $("p"); means "select all p elements".

Variables defined with let cannot be Redeclared.
Variables defined with let must be Declared before use.
Variables defined with let have Block Scope.

Variables declared with the var keyword can NOT have block scope.

Variables declared inside a { } block can be accessed from outside the block.

Redeclaring a JavaScript variable with var is allowed anywhere in a program:With let, redeclaring a variable in the same block is NOT allowed:
var x = 2;
// Now x is 2
var x = 3;
// Now x is 3
var x = 2;    // Allowed
let x = 3;    // Not allowed
{
let x = 2;    // Allowed
let x = 3     // Not allowed
}
{
let x = 2;    // Allowed
var x = 3     // Not allowed
}
Redeclaring a variable with let, in another block, IS allowed:
let x = 2;    // Allowed
{
let x = 3;    // Allowed
}
{
let x = 4;    // Allowed
}

For more information on Javascript refer to the links below:
[Developmozilla](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_is_JavaScript)
[W3Javascript](https://www.w3schools.com/js/default.asp)

