# Class 07: Object-Oriented Programming, HTML Tables

## Domain Modeling

### Explain why we need domain modeling

We need domain modeling for many reasons. The following a re three of these reasons:

* Performance optimization. Domain modeling allows instantiating of objects rather than the creation of new objects every time the code is run. Very useful for smaller devices like smart phones.
* Readability. Domain modeling allows readability of your code for other developers, or even yourself when you return to the code after many moons away.
* Reusability. Domain modeling enables code elements (i.e. classes) to be used throughout a project or in other projects.

## HTML Table Basics

### Why should tables not be used for page layouts

When tables are used for page layouts:

* they reduce accessibility functions for the visually impaired
* they reduce readability due to their more complex nature
* they are not automatically responsive. A lot of work must go into making them responsive

### List and describe 3 different semantic HTML elements used in an HTML `<table>`

* `<caption>`
* `<thead>`
* `<tbody>`

## Introducing Constructors

### What is a constructor and what are some advantages to using it?

In JavaScript, a constructor is a function used to create and initialize objects.

Some advantages of using a constructor are:

* Ability to create multiple instances of objects with similar properties and methods
* Code reusability
* Constructors allow you to encapsulate data and methods within an object, providing a level of data privacy.

### How does the term `this` differ when used in an object literal versus when used in a constructor?

In an object literal, `this` refers to the **object itself**. It is a reference to the object within which it is used.
`this` within an object literal context represents the current object, so its value is determined by the context in which it is used.
Example:

```js
const person = {
  name: 'Alice',
  greet: function() {
    console.log(`Hello, my name is ${this.name}.`);
  }
};

person.greet(); // "Hello, my name is Alice."
```

In a constructor function, `this` refers to the newly created instance of an object. When you use the `new` keyword to create an
object from a constructor, `this` **points to that new object**. `this` in a constructor context represents the **instance being created**.
Example:

```js
function Person(name) {
  this.name = name;
}

const person1 = new Person('Alice');
const person2 = new Person('Bob');

console.log(person1.name); // "Alice"
console.log(person2.name); // "Bob"

```

## Object Prototypes Using A Constructor

### Explain prototypes and inheritance via an analogy from your previous work experience

I once worked as a helpdesk employee assisting customers with their tech issues. I had a set of predefined documents and procedures to
solve common problems, such as resetting passwords, configuring email settings, and troubleshooting network connections.
These documents and procedures can be seen as "**prototypes**" in our analogy.

In this context, the "prototypes" are like manuals or guides that I used to resolve common issues. Each manual is tailored to a specific
type of problem. For example, there is a "Password Reset Manual," an "Email Configuration Manual," and a "Network Troubleshooting Manual."

These manuals served as templates for solving problems.

I had a colleague named Tony who was also part of the helpdesk team. Tony was new to the job and did not have all the manuals yet.
Instead of creating new manuals from scratch, he "inherited" some of my manuals. What this meant was that Tony could use the same procedures
and methods described in those manuals to solve related issues.

## Things I want to know more about

Nothing at the moment.
