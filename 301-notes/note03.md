# Class 03: Passing Functions as Props

## React Docs - lists and keys

### What does `.map()` return?

The `.map()` array method returns a new array by applying a provided function to each element of the array.

### If I want to loop through an array and display each value in JSX, how do I do that in React?

To loop through an array and display each value in JSX, you would use an array method that returns a new array, such as the `.map()` method.
For example:

```js
const listItems = products.map(product =>
  <li key={product.id}>
    {product.title}
  </li>
);

return (
  <ul>{listItems}</ul>
);
```

A more complete example:

```js
import React from 'react';

const MyComponent = () => {
  const myArray = ['Item 1', 'Item 2', 'Item 3'];

  return (
    <div>
      <h1>My Array Items:</h1>
      <ul>
        {myArray.map((item, index) => (
          <li key={index}>{item}</li>
        ))}
      </ul>
    </div>
  );
};

export default MyComponent;

```

Notice in both examples that a key is defined. This is required.

### Each list item needs a unique ____

Each list item needs a unique `key`.

### What is the purpose of a key?

The key attribute is used to provide a unique identifier for each rendered element.
It helps React efficiently update and re-render components when the array changes.

### The Spread Operator

### What is the spread operator?

The spread operator (`...`) is a syntax in JavaScript used for several purposes, particularly in array and object manipulations.
The spread operator expands an array into its elements.

### List 4 things that the spread operator can do

1. Create a new array by expanding one array inside of another array

   ```js
    const arr1 = [1, 2, 3];
    const arr2 = [...arr1, 4, 5, 6]; 
   ```

2. Create a shallow copy of an object, then add new key-value pairs:

   ```js
    const obj1 = { a: 1, b: 2 };
    const obj2 = { ...obj1, c: 3, d: 4 };
   ```

3. Spread elements of an array and pass them to a function as arguments:

   ```js
    const numbers = [1, 2, 3];

    function sum(x, y, z) {
    return x + y + z;
    }

    console.log(sum(...numbers));
   ```

4. Copying an array, rather than creating a reference to the original:

   ```js
    const arr = [1, 2, 3];
    const arr2 = [...arr]; // like arr.slice()

    arr2.push(4);
   ```

### Give an example of using the spread operator to combine two arrays

```js
const arr1 = [1, 2, 3];
const arr2 = [4, 5, 6];

const combinedArray = [...arr1, ...arr2];
```

### Give an example of using the spread operator to add a new item to an array

```js
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5, 6]; 
```

### Give an example of using the spread operator to combine two objects into one

```js
const obj1 = { a: 1, b: 2 };
const obj2 = { c: 3, d: 4 };

const combinedObject = { ...obj1, ...obj2 };
```

## How to Pass Functions Between Components

### In the video, what is the first step that the developer does to pass functions between components?

The first step that the developer takes to pass functions between components in React is to **define the function in the parent component**.
The next step is to pass it down to the child component as a **prop**.

### In your own words, what does the `handleClick` function do?

The `handleClick` function serves as a function that can be triggered in response to a button click event.

### How can you pass a method from a parent component into a child component?

To pass a method from a parent component to a child component, you must pass the method as a `prop`.

### How does the child component invoke a method that was passed to it from a parent component?

The child component invokes a method passed to it from a parent component by calling the method through the prop that received the function.

## Things I want to know more about

Nothing at the moment.
