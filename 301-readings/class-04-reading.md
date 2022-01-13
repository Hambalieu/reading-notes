# Readings: React and Forms.


## **Form**

## What is a ‘Controlled Component’?
>In React, mutable state is typically kept in the state property of components, and only updated with setState().An input form element whose value is controlled by React in this way is called a “controlled component”.


- Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
 >Storing user responses in a form as they are written rather than on submission allows for dynamic rendering for each input.

- How do we target what the user is entering if we have an event handler on an input field?
> User input can be targeted as a state of the component and invoked as properties of the component eig using  **this.state.value**.

 **The Conditional (Ternary) Operator Explained**

## Why would we use a ternary operator?

>A ternary operator allows you to assign one value to the variable if the condition is true, and another value if the condition is false. ... A ternary operator makes the assignment of a value to a variable easier to see, because it's contained on a single line instead of an if else block.


### Rewrite the following statement using a ternary statement:
- if(x===y){
  console.log(true);
} else {
  console.log(false);
}
- solution :
x===y ? console.log(true) : console.log(false);



## Below are the resources for this Note:

[React Forms](https://reactjs.org/docs/forms.html)

[The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)


## Things I want to know more about
- I want to know more about React Forms.
- I want to know more about ternary operator.
