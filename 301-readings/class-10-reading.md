# Readings: In memory storage

## Understanding the JavaScript Call Stack:
</br></br>

1. ## What is a ‘call’?
- A call is a Function invocation
</br></br>

2. ## How many ‘calls’ can happen at once?
- You can only do one (single) thing at a time.
</br></br>

3. ## What does LIFO mean?
- Last In,First Out. 
- It means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.
</br></br>


4. ## Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

       function      firstFunction(){
        console.log("Hello from firstFunction");
        }

       function secondFunction(){
         firstFunction();
         console.log("The end from secondFunction");
       }

       secondFunction();

**output**

- Hello from firstFunction
- The end from secondFunction


### This is what happens when the code is run:
1. When `secondFunction()` gets executed, an empty stack frame is created. It is the main (anonymous) entry point of the program.
2. `secondFunction()` then calls `firstFunction()`which is pushed into the stack.
3. `firstFunction()` returns and prints `“Hello from firstFunction”` to the console.
4. `firstFunction()` is pop off the stack.
5. The execution order then move to `secondFunction()`.
6. `secondFunction()` returns and print `“The end from secondFunction”` to the console.
7. `secondFunction()` is pop off the stack, clearing the memory.

[callstack]()

</br></br>

5. ## What causes a Stack Overflow?
- A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point

</br></br>

## JavaScript error messages.


1. ## What is a ‘refrence error’?
- This is as simple as when you try to use a variable that is not yet declared you get this type os errors.e.g
`console.log(foo) // Uncaught ReferenceError: foo is not defined`
</br></br>

2. ## What is a ‘syntax error’?
- this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.e.g
`JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1`
</br></br>

3. ## What is a ‘range error’?
- Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.e.g
`var foo= []`
`foo.length = foo.length -1 // `
`Uncaught RangeError: Invalid array length`
</br></br>

4. ## What is a ‘tyep error’?
- Show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.e.g
`var foo = {}`
`foo.bar //` `undefined`
`foo.bar.baz // `
`Uncaught TypeError: Cannot read property` `'baz' of undefined`       
</br></br>


5. ## What is a breakpoint?
- Putting a debugger statement in your code in the line you want to break.
</br></br>


6. ## What does the word ‘debugger’ do in your code?
- A Debugger is used to identify coding errors at various development stages.

</br></br>

## References/Citations

[Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)
</br></br>


[JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

## Things I want to know more about
- I would like to learn more about call stack
