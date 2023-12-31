# Class 03: HTML Lists, Control Flow with JS, and the CSS Box Model

![JavaScript Image](../images/JavaScript-code.jpg)

As a software developer, understanding the basics of HTML, CSS, and JavaScript is fundamental and foundational. HTML (Hypertext Markup Language) provides the structure and content of web pages, serving as the backbone of the web. CSS (Cascading Style Sheets) enables you to control the presentation and layout, making content visually appealing and responsive. JavaScript, on the other hand, is a versatile scripting language that adds interactivity and dynamic behavior to web applications. Together, these technologies form the core of modern web development. Proficiency in HTML, CSS, and JavaScript empowers software developers to create and customize web interfaces, ensuring a seamless user experience. As web technologies increasingly integrate with various software platforms and technologies, a strong grasp of these fundamentals becomes a valuable asset in the broader software development landscape.

## When should you use an unordered list in your HTML document?

You would use an unordered list when grouping a collection of items that do not have a numerical order or relationship to each other.

## How do you change the bullet style of unordered list items?

To change the bullet style of unordered list items, you would use the `type` attribute.

## When should you use an ordered list vs an unordered list in your HTML document?

You should use an ordered list of the numerical order of the list is meaningful. If changing the order of the list does not change the meaning, then an unordered list should be used.

## Describe two ways you can change the numbers on list items provided by an ordered list?

Two ways to change the numbers on list items in n ordered list are:

1. using the `type` attribute to change the numbering type (i.e., lowercase letters, Roman numerals, etc.).
2. using the `start` attribute to select which number or numeral to start from.

## Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?

> In the whimsical tale of "The Box Model," Margin and Padding play the roles of two inseparable characters who define the personal space and interactions within the story's world. Margin, always courteous and respectful, represents the outermost boundaries, providing the characters with a sense of personal space, preventing overcrowding, and maintaining harmony among elements. On the other hand, Padding, the warm and welcoming character, resides within, offering comfort and a protective barrier to the content, ensuring it doesn't get too close to the edges. Together, they balance the spatial dynamics in the tale, creating an enchanting narrative where every element finds its place and maintains a sense of harmony and order in the storytelling world of web design.

* *(Utilized ChatGPT assistance)*

## List and describe the four parts of an HTML elements box as referred to by the box model

* **Content** box - area of space where content is rendered/displayed
* **Padding** box - padding space around the edge of the content box
* **Border** box - border space around the edge of the padding box
* **Margin** box - outermost area that wraps around all other areas and sits between the element and other elements

## What data types can you store inside of an Array?

JavaScript arrays are versatile and can contain **strings**, **numbers**, **objects**, **functions**, and even other **arrays**.

## Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?

```js
const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
```

Yes, the above `people` array is valid due to the versatility of JavaScript arrays.
To access the values stored in this array, you would need to access the index of the first level array, then the index of the nested, second level array. For example:

```js
console.log(people[0][0]);
// Will output 'pete'
// 3 arrays inside of the people `array`, with each array containing 4 values
// Also know as a two-dimensional array 
```

## List five shorthand operators for assignment in javascript and describe what they do

Five shorthand operators for assignment in javascript:

* `x += f()` => Addition assignment operator that increments `x` by the value of `f()`.
* `x -= f()` => Subtraction assignment operator that decrements `x` by the value of `f()`.
* `x *= f()` => Multiplication assignment operator that multiplies `x` by `f()`, then assigns the product back to `x`.
* `x /= f()` => Division assignment operator that divides `f()` by the original value of `x`, then assigns the new value back to `x`.
* `x++` => Addition assignment operator that increments the value of `x` by `1`.

## Read the code below, evaluate the last expression, and explain what the result would be and why

```js
 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;
```

The code above would evaluate to `10dog`. Explanation:

* First, evaluates the expression inside the parentheses by converting `false` to 0, then adding `10 + 0`
* Next, it does a type coercion of the number `10` into a string since the variable `b` is a string
* Finally, it concatenates the string `"10"` and the string `"dog"` to output the value `10dog`

## Describe a real world example of when a conditional statement should be used in a JavaScript program

A real world example of when a conditional statement should be used in JavaScript is when building an examination program.
In this type of program, a is given a number of choices per each question, with one or more correct answers.
If the user chooses the correct answer, the points alloted for that answer is added to the user's overall score.
If the user chooses the wrong answer, no points are added to the users overall score.
At the conclusion of the test, the program would then calculate the user score and output a grade.

## Give an example of when a Loop is useful in JavaScript

A useful example of a JavaScript loop would be a program that calculates a set of numerical values and outputs the sum, or product when a condition is met.

## Things I want to know more about

I would like to know more about recursive functions and the best method of implementation.
