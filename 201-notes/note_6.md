# Problem Domain, Objects, and the DOM

## JavaScript Object Basics

### How would you describe an object to a non-technical friend you grew up with?

Think of a JavaScript object like a container or a box with different compartments, where each compartment can hold something.
Each compartment has a label on it, so you know what's inside.

Say you have an object called "Car." Inside this object, you can have compartments like "Color," "Make," "Model," and "Year."
In the "Color" compartment, you might have "Blue." In the "Make" compartment, you could have "Toyota." And so on.

The JavaScript object is like a handy way to group related information together. It's just like organizing your stuff in different
compartments to keep everything in order. You can access the information in these compartments easily, and it helps make your code
more organized and understandable.

### What are some advantages to creating object literals?

### How do objects differ from arrays?

### Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.

### Evaluate the code below. What does the term this refer to and what is the advantage to using this?

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

## Introduction To The DOM

### What is the DOM?

### Briefly describe the relationship between the DOM and JavaScript.

## Things I want to know more about
