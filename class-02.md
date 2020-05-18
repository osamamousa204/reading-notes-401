## Inheritance with the prototype chain

All JavaScript objects inherit properties and methods from a prototype.

To add a new property to a constructor, i must add it to the constructor function.

## Prototype Inheritance

All JavaScript objects inherit properties and methods from a prototype:
ex:
Date objects inherit from Date.prototype
Array objects inherit from Array.prototype
Person objects inherit from Person.prototype
The Object.prototype is on the top of the prototype inheritance chain:

Date objects, Array objects, and Person objects inherit from Object.prototyp

## Adding Properties and Methods to Objects
Sometimes i want to add new properties (or methods) to all existing objects of a given type.

Sometimes i want to add new properties (or methods) to an object constructor.


### this keyword :A property of an execution context (global, function or eval) that, in non–strict mode, is always a reference to an object and in strict mode can be any value.

A function's this keyword behaves a little differently in JavaScript compared to other languages. It also has some differences between strict mode and non-strict mode.

In most cases, the value of this is determined by how a function is called (runtime binding). It can't be set by assignment during execution, and it may be different each time the function is called. ES5 introduced the bind() method to set the value of a function's this regardless of how it's called, and ES2015 introduced arrow functions which don't provide their own this binding (it retains the this value of the enclosing lexical context).

## JavaScript Classes

Use the keyword `class` to create a class, and always add the `constructor()` method.

The constructor method is called each time the class object is initialized.

### Methods

The constructor method is special, it is where we initialize properties, it is called automatically when a class is initiated, and it has to have the exact name "constructor", in fact, if i do not have a constructor method, JavaScript will add an invisible and empty constructor method.

### Inheritance
To create a class inheritance, use the `extends` keyword.

A class created with a class inheritance inherits all the methods from another class.

### Errors

Applications running in Node.js will generally experience four categories of errors:

Standard JavaScript errors such as:

`<EvalError>` : thrown when a call to eval() fails.
`<SyntaxError>` : thrown in response to improper JavaScript language syntax.
`<RangeError>` : thrown when a value is not within an expected range
`<ReferenceError>` : thrown when using undefined variables
`<TypeError>` : thrown when passing arguments of the wrong type
`<URIError>` : thrown when a global URI handling function is misused.
System errors triggered by underlying operating system constraints such as attempting to open a file that does not exist, attempting to send data over a closed socket, etc;
And User-specified errors triggered by application code.













[Home Page](https://osamamousa204.github.io/reading-notes-401/)
