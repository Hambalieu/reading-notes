#  Arrays, Loops, Imports

## Packages
- **Package** = **directory**. Java classes can be grouped together in packages. A package name is the same as the directory (folder) name which contains the .java files. You declare packages when you define your Java program, and you name the packages you want to use from other libraries in an import statement.

## Common imports examples
- import java.awt.*;	Common GUI elements.
- import java.awt.event.*;	The most common GUI event listeners.
- import javax.swing.*;	More common GUI elements. Note "javax".
- import java.util.*;	Data structures (Collections), time, Scanner, etc classes.
- import java.io.*;	Input-output classes.
- import java.text.*;	Some formatting classes.
- import java.util.regex.*;	Regular expression classes.

### Import Notes on FAQ:
1. -Q: I've imported java.awt.*, why do I also need java.awt.event.*?
   -A: The wildcard "*" only makes the classes in this package visible, not any of the subpackages.
2. -Q: Why don't I need an import to use String, System, etc?
   -A: All classes in the java.lang package are visible without an import.


## LOOPS

### For Loop
- A *for loop* is a control structure that allows us to repeat certain operations by incrementing and evaluating a loop counter.
## Examples of for loops are :
- Simple or Enhanced for loop
#### example of a simple for loop 
- >>for (int i = 0; i < 5; i++) {
  System.out.println("Simple for loop: i = " + i);
  }
#### example of an Enhanced  for loop
- >>int[] intArr = { 0,1,2,3,4 };
  for (int num : intArr) {
  System.out.println("Enhanced for-each loop: i = " + num);
  }

### Iterable.forEach()
- ####Example of forEach()
>>List<String> names = new ArrayList<>();
names.add("Larry");
names.add("Steve");
names.add("James");
names.add("Conan");
names.add("Ellen");
names.forEach(name -> System.out.println(name));


## WHILE LOOP
- The while loop is Java's most fundamental loop statement. It repeats a statement or a block of statements while its controlling Boolean-expression is true.
- **The loop's Boolean-expression is evaluated before the first iteration of the loop** – which means that if the condition is evaluated to false, the loop might not run even once.
#### Example of while loop 
- >>int i = 0;
  while (i < 5) {
  System.out.println("While loop: i = " + i++);
  }
  
## Do-While LOOP
- The do-while loop works just like the while loop except for the fact that **the first condition evaluation happens after the first iteration of the loop**.
#### Example of a do-while loop
- >>int i = 0;
  do {
  System.out.println("Do-While loop: i = " + i++);
  } while (i < 5);

###  References/Citations
[Packages And Import](https://perso.ensta-paris.fr/~diam/java/online/notes-java/language/10basics/import.html)
[LOOPS](https://www.baeldung.com/java-loops)