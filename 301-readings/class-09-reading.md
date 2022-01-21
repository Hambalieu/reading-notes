# Readings: Functional Programming.

<br></br>

1. ## What is functional programming?
- Functional programming is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects. Functional programming is declarative rather than imperative, and application state flows through pure functions

<br></br>

2. ## What is a pure function and how do we know if something is a pure function?
- A pure function is a function which:
Given the same inputs, always returns the same output, and Has no side-effects.

<br></br>

3. ## What are the benefits of a pure function?
- Pure functions are much easier to read and reason about.
- We can quickly understand a function and its dependencies, just by reading the function's declaration.
- They are easy to test and refactor.

<br></br>

4. ## What is immutability?
- Immutability is a central concept of functional programming because without it, the data flow in your program is lossy. State history is abandoned, and strange bugs can creep into your software


<br></br>

5. ## What is Referential transparency?
-  You can replace a function call with its resulting value without changing the meaning of the program. 

<br></br>

# Node JS Tutorial for Beginners #6 - Modules and require().

<br></br>

1. ## What is a module?
- Is another JavaScript file in our Node Js .Instead of having all our code in App.js we create modules (Js files ) for all certain code in our app.js.
<br></br>

2. ## What does the word ‘require’ do?
- We use require  to pass through the the path to the module that we require in our app.js.
<br></br>

3. ## How do we bring another module into the file the we are working in?
- We create a path for the module into our current file we working on .`e.g. './<filename>'`.
<br></br>

4. ## What do we have to do to make a module available?

-We have to `module.export= <whatever we want to use from the module>`


</br></br>

## References/Citations

[Functional Programming](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa))
</br></br>


[Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)
