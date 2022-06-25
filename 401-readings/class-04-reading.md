## OOP
### Objetcs 
- Objects has State and Behavior e.g of a real world object A dog has a state of name or color or breed and a behavior of barking ,fetching and wagging tail.
- An object stores its state in fields (variables in some programming languages) and exposes its behavior through methods (functions in some programming languages).
- Java Program creates many objects which are invoke using methods
###Bundling code into individual software objects provides a number of benefits, including:
1. Modularity: The source code for an object can be written and maintained independently of the source code for other objects. Once created, an object can be easily passed around inside the system.
2. Information-hiding: By interacting only with an object's methods, the details of its internal implementation remain hidden from the outside world.
3. Code re-use: If an object already exists (perhaps written by another software developer), you can use that object in your program. This allows specialists to implement/test/debug complex, task-specific objects, which you can then trust to run in your own code.
4. Pluggability and debugging ease: If a particular object turns out to be problematic, you can simply remove it from your application and plug in a different object as its replacement. This is analogous to fixing mechanical problems in the real world. If a bolt breaks, you replace it, not the entire machine.

### Classes 
- A class is the blueprint from which individual objects are created.
- the first letter of a class name should be capitalized, and
- the first (or only) word in a method name should be a verb.
#### Declaring a class
> class MyClass {
// field, constructor, and
// method declarations
} 
#### Access Modifiers 
- **public** modifier—the field is accessible from all classes.
- **private** modifier—the field is accessible only within its own class.

###Methods
- Here is an example of a typical method declaration:
- > public double calculateAnswer(double wingSpan, int numberOfEngines,
  double length, double grossTons) {
  //do the calculation here
  }
- The only required elements of a method declaration are the method's return type, name, a pair of parentheses, (), and a body between braces, {}.
- The return type—the data type of the value returned by the method, or **void** if the method does not return a value.


#### Providing Constructors for our Classes
-A class contains constructors that are invoked to create objects from the class blueprint.
-Constructor declarations look like method declarations—except that they use the name of the class and have no return type.

#### Parameters 
-**Parameters** refers to the list of variables in a method declaration
- **Arguments** are the actual values that are passed in when the method is invoked.
- You can use any data type for a parameter of a method or a constructor.
- If you want to pass a method into a method, then use a **lambda** expression or a method reference.

1. **Declaration**: The code set in bold are all variable declarations that associate a variable name with an object type
2. **Instantiation**: The new keyword is a Java operator that creates the object.
> Point originOne = new Point(23, 94);
4. **Initialization**: The new operator is followed by a call to a constructor, which initializes the new object.


### Decimal Binary AND Hexadecimal numbers
- The Decimal Number System is also called "Base 10", because it is based on the number 10
- Binary Numbers are just "Base 2" instead of "Base 10". So you start counting at 0, then 1, then you run out of digits ... so you start back at 0 again, but increase the number on the left by 1.
- Hexadecimal numbers are interesting. There are 16 of them!
They look the same as the decimal numbers up to 9, but then there are the letters ("A',"B","C","D","E","F") in place of the decimal numbers 10 to 15.
So a single Hexadecimal digit can show 16 different values instead of the normal 10 like this:
>Decimal:	0	1	2	3	4	5	6	7	8	9	10	11	12	13	14	15
Hexadecimal:	0	1	2	3	4	5	6	7	8	9	A	B	C	D	E	F

## Reference and Citations
[Object and Class](https://docs.oracle.com/javase/tutorial/java/concepts/object.html)          
[Classes](https://docs.oracle.com/javase/tutorial/java/javaOO/classes.html)             
[Binary,Decimal and Hexadecimal Numbers](https://www.mathsisfun.com/binary-decimal-hexadecimal.html)           
