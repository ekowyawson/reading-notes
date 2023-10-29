# Problem Domain, Objects, and the DOM

## JavaScript Object Basics

### How would you describe an object to a non-technical friend you grew up with?

A JavaScript object is like a container or a box with different compartments, where each compartment can hold something.
Each compartment has a label on it, so you know what's inside.

Say you have an object called "Car." Inside this object, you can have compartments like "Color," "Make," "Model," and "Year."
In the "Color" compartment, you might have "Blue." In the "Make" compartment, you could have "Toyota." And so on.

The JavaScript object is like a handy way to group related information together. Similar to organizing your things in different
compartments to keep everything in order. You can access the information in these compartments easily, and it helps make your code
more organized.

### What are some advantages to creating object literals?

An object literal is enclosed in curly braces `{}` and consists of key-value pairs, where keys are strings that act as property names,
and values can be any valid JavaScript data type, including other objects, or functions.

Object literals differ from objects instantiated from classes.

Advantages of creating object literals are:

* Object literals provide a simple and concise way to define objects with key-value pairs
* They are JSON (JavaScript Object Notation) compatible (my favorite way of presenting date in API's)
* No need to create classes for objects and instantiate them (if not using dynamic content)

### How do objects differ from arrays?

Arrays are singular items identified by an index or indices, whereas an object can contain grouped items, identified by keys, and hold values.

* **Array**:

```js
const someArray = ['this', 'that', 'and', 'the', 'third'];
```

* **Object**

```js
const person = {
  firstName: "John",
  lastName: "Doe"
};
```

### Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation

In JavaScript, you typically use dot notation to access an object's properties.
However, some situations may require bracket notation as a necessary or more appropriate use case.
Examples of these cases include, but are not limited to:

* When you need to access an object's property dynamically (based on a variable or an expression)
* If an object's property name includes special characters
* If the property name is not a valid JavaScript identifier (e.g., contains spaces or starts with a digit)

### Evaluate the code below. What does the term `this` refer to and what is the advantage to using this?

```js
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
```

In the code above, `this` refers to the current object, which, in this case, is the dog object.
The `this` keyword is used to access properties and methods within the context of the current object.

The main advantage of using the `this` JavaScript keyword is that it allows dynamic access to contents in the object
(you don't have to use `dog.name` every time, especially with the variable changes to something like `cat`).

## Introduction To The DOM

### What is the DOM?

**DOM** stands for Document Object Model and is considered the Application Programming Interface (API) for web documents.
It allows programs to change the web document structure, style, and content by presenting it to the program... programmatically.

### Briefly describe the relationship between the DOM and JavaScript

The DOM is a representation of the structure and content of a web page in the form of a tree-like structure.
Each element on a web page, such as HTML tags, is represented as a node in this tree. JavaScript can interact with the DOM,
allowing your code to access and manipulate the content and structure of a web page dynamically. JavaScript can modify the
properties and attributes of DOM elements, respond to user interactions, and update the page without requiring a full page refresh.

## Things I want to know more about

I want to better understand the JavaScript fetch API and how to easily and dynamically present fetched data within the DOM.
