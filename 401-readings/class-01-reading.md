# Java Basics
## Variables 
- The term "instance variable" is another name for non-static field.
- The term "class variable" is another name for static field.
- A local variable stores temporary state; it is declared inside a method.
- A variable declared within the opening and closing parenthesis of a method is called a parameter.
- What are the eight primitive data types supported by the Java programming language? **byte**, **short**, **int**, **long**, **float**, **double**, **boolean**, **char**
- Character strings are represented by the class java.lang.String.
- Array is a container object that holds a fixed number of values of a single type.

## Operators

### Simple Assignment Operator (=)
### Arithmetic Operators
- (+) Additive operator (also used
for String concatenation)
- (-) Subtraction operator
- (*) Multiplication operator
- (/) Division operator
- (%) Remainder operator

### Unary Operators
- (+) Unary plus operator; indicates
  positive value (numbers are
  positive without this, however)
- (-) Unary minus operator; negates
  an expression
- (++) Increment operator; increments
  a value by 1
- (--) Decrement operator; decrements
  a value by 1
- (!)  Logical complement operator;
  inverts the value of a boolean

### Equality and Relational Operators

- (==)     Equal to
- (!=)     Not equal to
- (>)     Greater than
- (>=)    Greater than or equal to
- (<)       Less than
- (<=)     Less than or equal to

### Conditional Operators
- &&      Conditional-AND
- ||      Conditional-OR
- ?:      Ternary (shorthand for
*if-then-else* statement)

### Bitwise and Bit Shift Operators

- ~       Unary bitwise complement
- <<      Signed left shift
- (>>)      Signed right shift
- (>>>)     Unsigned right shift
- &       Bitwise AND
- ^       Bitwise exclusive OR
- |       Bitwise inclusive OR

#### Expressions, Statements, and Blocks
1. Operators may be used in building expressions, which compute values
2. Expressions are the core components of **statements**.
3. Statements may be grouped into **blocks**.
4. The following code snippet is an example of a compound expression.
   >>1 * 2 * 3
5. Statements are roughly equivalent to sentences in natural languages, but instead of ending with a period, a statement ends with a **semicolon**.
6. A block is a group of zero or more statements between balanced **braces** and can be used anywhere a single statement is allowed.

### Examples 
>> aValue = 8933.234; // assignment statement
>> aValue++; // increment statement
>> System.out.println("Hello World!"); // method invocation statement
>> Bicycle myBike = new Bicycle(); // object creation statement

### Control Flow Statements
- The *if-then* statement is the most basic of all the control flow statements. It tells your program to execute a certain section of code only if a particular test evaluates to *true*.
- The *if-then-else* statement provides a secondary path of execution when an "if" clause evaluates to *false*.
- The *switch* statement allows for any number of possible execution path
- The *while* and *do-while* statements continually execute a block of statements while a particular condition is *true*.
- The difference between *do-while* and *while* is that *do-while* evaluates its expression at the bottom of the loop instead of the top.
- The statements within the *do* block are always executed at least once
- The *for* statement provides a compact way to iterate over a range of values.



[Java Basic](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html)
[Reading Java Documentation](https://www.dummies.com/category/articles/java-33602)
[Good read on what is java compiling](https://www.reddit.com/r/explainlikeimfive/comments/233dq5/eli5_what_does_it_mean_to_compile_code/)
