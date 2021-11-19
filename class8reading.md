Read: 08 - Operators and Loops:

Loop and Iteration:

-Loops offer a quick and easy way to do something repeatedly.

for statement
A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.

A for statement looks as follows:

for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement

  When a for loop executes, the following occurs:

The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. If the value of condition is false, the for loop terminates. (If the condition expression is omitted entirely, the condition is assumed to be true.)
The statement executes. To execute multiple statements, use a block statement ({ ... }) to group those statements.
If present, the update expression incrementExpression is executed.
Control returns to Step 2.


do...while statement
The do...while statement repeats until a specified condition evaluates to false.
A do...while statement looks as follows:

do
  statement
while (condition);

Example
In the following example, the do loop iterates at least once and reiterates until i is no longer less than 5.
let i = 0;
do {
  i += 1;
  console.log(i);
} while (i < 5);


while statement
A while statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:
while (condition)
  statement

break statement
Use the break statement to terminate a loop, switch, or in conjunction with a labeled statement.

When you use break without a label, it terminates the innermost enclosing while, do-while, for, or switch immediately and transfers control to the following statement.
When you use break with a label, it terminates the specified labeled statement.
The syntax of the break statement looks like this:

break;
break [label];
The first form of the syntax terminates the innermost enclosing loop or switch.
The second form of the syntax terminates the specified enclosing labeled statement.



Operators:
JavaScript has both binary and unary operators, and one special ternary operator, the conditional operator. A binary operator requires two operands, one before the operator and one after the operator:

Binary operator: 3+5 or x*y
unary oprator: ++x or x++


Expressions
An expression is any valid unit of code that resolves to a value.

Every syntactically valid expression resolves to some value but conceptually, there are two types of expressions: with side effects (for example: those that assign value to a variable) and those that in some sense evaluate and therefore resolve to a value.

The expression x = 7 is an example of the first type. This expression uses the = operator to assign the value seven to the variable x. The expression itself evaluates to seven





A complete and detailed list of operators and expressions is also available in the reference link below :
[OperatorsList](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators)


For more infomation please refer to the links below:
[EperaorsandExpressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators) 

[Loops](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)