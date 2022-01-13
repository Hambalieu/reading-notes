# Readings: Passing Functions as Props:

## What does .map() return?
- The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.

## If I want to loop through an array and display each value in JSX, how do I do that in React?
- Save the return value calling the map method on the array in question and instantiate elements, inserting elements of the array within the map function


## Each list item needs a unique ____.
- Key

## What is the purpose of a key?
- The purpose of keys is to help React keep track of which items that have been changed.

# The Spread Operator

## What is the spread operator?
- The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

## List 4 things that the spread operator can do.
 - Adding to state in React
 - Using an array as arguments.
 - Copying an array.
 - Concatenating or combining arrays.


 ## Give an example of using the spread operator to combine two arrays.

 > - const arr1 = [1,2,3]
  > - const arr2 = [4,5,6]
  > - const arr3 = [... arr1, ... arr2] //arr3 ==> [1,2,3,4,5,6]

## Give an example of using the spread operator to add a new item to an array.

 > - let numberStore = [0, 1, 2];
 > - let newNumber = 12;
 > - numberStore = [...numberStore, newNumber];

## Give an example of using the spread operator to combine two objects into one.

 > - const person = { name: 'David Walsh', gender: 'Male' };
  > - const tools = { computer: 'Mac', editor: 'Atom' };
  > - const summary = {...person, ...tools};



# How to Pass Functions Between Components:

## In the video, what is the first step that the developer does to pass functions between components?
- The developer passes the function to the child component using props and referencing this.functionName.

## In your own words, what does the increment function do?
- The increment function updates the state object.

## How can you pass a method from a parent component into a child component?
- You can pass methods from parents component into child component using props.

## How does the child component invoke a method that was passed to it from a parent component?
- A child component can call a method passed to it by using: this.props.methodName()


## Below is the Source Links and Video :
[List and Keys](https://reactjs.org/docs/lists-and-keys.html)

[Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

[React - How to Pass Functions between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)




## Things I want to know more about

-I want to learn more about the spread Operator.
