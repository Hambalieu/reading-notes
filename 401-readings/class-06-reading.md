# Inheritance and Interfaces

##Objects 
- Real-world objects contain **state** and **behavior**.
- A software object's state is stored in **fields**.
- A software object's behavior is exposed through **methods**.
##Classes
- A blueprint for a software object is called a **class**.
## Interface 
- an interface is a group of related methods with empty bodies.
- If your class claims to implement an interface, all methods defined by that interface must appear in its source code before the class will successfully compile.
- Interfaces cannot be instantiated—they can only be implemented by classes or extended by other interfaces.
- To declare a class that implements an interface, you include an **implements** clause in the class declaration.
- An interface declaration can contain method signatures, default methods, static methods and constant definitions.
- An interface name can be used anywhere a type can be used

##Inheritance 
- Object-oriented programming allows classes to inherit commonly used state and behavior from other classes.
- Except for the Object class, a class has exactly one direct superclass.
- A class inherits fields and methods from all its superclasses, whether direct or indirect
- A subclass can override methods that it inherits, or it can hide fields or methods that it inherits
- You can prevent a class from being subclassed by using the final keyword in the class's declaration.
- You can prevent a method from being overridden by subclasses by declaring it as a final method.
- An abstract class can only be subclassed; it cannot be instantiated.
- An abstract class can contain abstract methods—methods that are declared but not implemented. Subclasses then provide the implementations for the abstract methods

### Notes:
- publicly exposed methods is known as data **encapsulation**.
- Common behavior can be defined in a **superclass** and inherited into a **subclass** using the **extends** keyword.
- A collection of methods with no implementation is called an **interface**.
- A namespace that organizes classes and interfaces by functionality is called a **package**.
- he term API stands for **Application Programming Interface**.


## Reference and Citations
[Java OO Tutorial (review Object and Class, read the rest)](https://docs.oracle.com/javase/tutorial/java/concepts/)
[Java Inheritance & Interfaces Tutorial](https://docs.oracle.com/javase/tutorial/java/IandI/index.html)