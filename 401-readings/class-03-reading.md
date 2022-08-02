# Read: 03 - Maps, primitives, File I/O

## Java Type System
- Java has a two-fold type system consisting of primitives such as int, boolean and reference types such as Integer, Boolean.
- The process of converting a primitive type to a reference one is called autoboxing
- While the process of converting reference types to primitive types is called unboxing.
- >>Integer j = 1;          // autoboxing
  int i = new Integer(1); // unboxing

#### The Primitive types have the following impact on memory.
- boolean – 1 bit
- byte – 8 bits
- short, char – 16 bits
- int, float – 32 bits
- long, double – 64 bits
#### The reference types impact on memory using the wrapper class
- Boolean – 128 bits
- Byte – 128 bits
- Short, Character – 128 bits
- Integer, Float – 128 bits
- Long, Double – 192 bits

> We can see that a single variable of Boolean type occupies as much space as 128 primitive ones, while one Integer variable occupies as much space as four int ones.
> the primitive types are much faster and require much less memory
> the objects in Java are slower and have a bigger memory impact than their primitive analogs.
> Surprisingly, arrays of the primitive types long and double consume more memory than their wrapper classes Long and Double.
## Exceptions
- A program can use exceptions to indicate that an error occurred.
- To throw an exception, use the **throw** statement.
- A method that throws an uncaught, checked exception must include a **throws** clause in its declaration.
- The class of the exception object indicates the type of exception thrown.
- The exception object can contain further information about the error, including an error message
- With exception chaining, an exception can point to the exception that caused it, which can in turn point to the exception that caused it, and so on

### Try ,Catch ,finally
- The **try** block identifies a block of code in which an exception can occur.
- The **catch** block identifies a block of code, known as an exception handler, that can handle a particular type of exception.
- The **finally** block identifies a block of code that is guaranteed to execute, and is the right place to close files, recover resources, and otherwise clean up after the code enclosed in the try block.
> The try statement should contain at least one catch block or a finally block and may have multiple catch blocks.

## Scanner
- Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type

### Path 
#### Relative Path
>An absolute path always contains the root element and the complete directory list required to locate the file. For example, /home/sally/statusReport is an absolute path. All of the information needed to locate the file is contained in the path string.
#### Absolute Path
>A relative path needs to be combined with another path in order to access a file. For example, joe/foo is a relative path. Without more information, a program cannot reliably locate the joe/foo directory in the file system.

### File 
> The Files class is the other primary entrypoint of the java.nio.file package.


## Reference and Citation
[Java Primitives versus Objects](https://www.baeldung.com/java-primitives-vs-objects)          
[Exceptions](https://docs.oracle.com/javase/tutorial/essential/exceptions/summary.html)          
[File I/O scanner stream](https://docs.oracle.com/javase/tutorial/essential/io/scanning.html)                   
