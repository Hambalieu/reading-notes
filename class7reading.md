#Read: 07 - Programming with JavaScript:

Control  Flow:
The control flow is the order in which the computer executes statements in a script.

Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops.

For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else, so that different code executes depending on whether the form is complete or not:

if (field==empty) {
    promptUser();
} else {
    submitForm();
}

A typical script in JavaScript includes many control structures,including conditionals,loops and functions.


 JavaScript Functions:

 A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

 -Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).
 -The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)
-The code to be executed, by the function, is placed inside curly brackets: {}

-function name(parameter1, parameter2, parameter3) {
  // code to be executed
}

Function Return:
-When JavaScript reaches a return statement, the function will stop executing.
-If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

Code Example:
let x = myFunction(4, 3);   // Function is called, return value will end up in x

function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
}
The result in x will be:
12

-Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations.

-Since local variables are only recognized inside their functions, variables with the same name can be used in different functions.

-Local variables are created when a function starts, and deleted when the function is completed.


JavaScript Operators:

Assign values to variables and add them together:
let x = 5;         // assign the value 5 to x
let y = 2;         // assign the value 2 to y
let z = x + y;     // assign the value 7 to z (5 + 2)

JavaScript Arithmetic Operators
Arithmetic operators are used to perform arithmetic on numbers:
Operator	Description
+	Addition
-	Subtraction
*	Multiplication
**	Exponentiation (ES2016)
/	Division
%	Modulus (Division Remainder)
++	Increment
--	Decrement

Assignment operators assign values to JavaScript variables.

Operator	Example	Same As
=	x = y	x = y
+=	x += y	x = x + y
-=	x -= y	x = x - y
*=	x *= y	x = x * y
/=	x /= y	x = x / y
%=	x %= y	x = x % y
**=	x **= y	x = x ** y


The + operator can also be used to add (concatenate) strings.

-Example
let text1 = "John";
let text2 = "Doe";
let text3 = text1 + " " + text2;
The result of text3 will be:
John Doe

-Example
let text1 = "What a very ";
text1 += "nice day";
The result of text1 will be:
What a very nice day


Adding two numbers, will return the sum, but adding a number and a string will return a string:
Example
let x = 5 + 5;
let y = "5" + 5;
let z = "Hello" + 5;

JavaScript Comparison Operators
Operator	Description
==	equal to
===	equal value and equal type
!=	not equal
!==	not equal value or not equal type
>	greater than
<	less than
>=	greater than or equal to
<=	less than or equal to
?	ternary operator


JavaScript Logical Operators
Operator	Description
&&	logical and
||	logical or
!	logical not


JavaScript Type Operators
Operator	Description
typeof	Returns the type of a variable
instanceof	Returns true if an object is an instance of an object type

JavaScript Bitwise Operators
Bit operators work on 32 bits numbers.

Any numeric operand in the operation is converted into a 32 bit number. The result is converted back to a JavaScript number.
Operator	Description	Example	Same as	Result	Decimal
&	AND	5 & 1	0101 & 0001	0001	 1
|	OR	5 | 1	0101 | 0001	0101	 5
~	NOT	~ 5	 ~0101	1010	 10
^	XOR	5 ^ 1	0101 ^ 0001	0100	 4
<<	Zero fill left shift	5 << 1	0101 << 1	1010	 10
>>	Signed right shift	5 >> 1	0101 >> 1	0010	  2
>>>	Zero fill right shift	5 >>> 1	0101 >>> 1	0010	  2
  
For more information on Javascript refer to the links below:
[Control Flow](https://developer.mozilla.org/en-US/docs/Glossary/Control_flow)
[Functions](https://www.w3schools.com/js/js_functions.asp)
[Operations](https://www.w3schools.com/js/js_operators.asp)



