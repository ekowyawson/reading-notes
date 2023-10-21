# Class 01 - Setup Developer Toolbelt

The journey into any area in modern technology, as a professional, always begins with an introduction to toolkits and toolkit setup (both hardware and software). This introduction forms a fundamental basis that allows all learners to start from a baseline and easily progress. In software development, these toolkits comprise more of (you guessed it) software that are essential to accomplishing the specific tasks required of the profession. The most essential tool in software development, however, is knowledge of the fundamentals.

This article will delve into the fundamentals of web development; how the web works and the tools used to make it work.

## A short poem describing how HTTP sends data between computers

In cyberspace, where connections race,
HTTP zooms, in steady haste.
A protocol of data's flight,
From a client to distant site.

With every click, a request is sent,
To fetch a page, from a server’s ‘tent.
Through cables, wires, and DNS,
Information finds its destined rest.

Request and response, a cyber fancy,
Through servers, routers, the data dances.
Each packet, a note in the grand ballet,
HTTP hosts the internet's soiree.

From client's call to server's embrace,
HTTP's a link in the web's embrace.
In ones and zeros, it weaves its spell,
The language of the net flows so well.

## How HTML, CSS, and JS files are “parsed” in the browser

When you send a **request** from your browser (by visiting a page or clicking a link) to a server on the internet, it sets off a hierarchal order of operations. This order of operations ends with your browser eventually receiving the requested data, then **parsing** that data to display the webpage/content you requested. Here, parsing refers to your browser reading the coded elements sent by the responding server as instructions, then using those instructions to render the web page/content. Let’s look at the order data is parsed when your web browser receives the data from the server:

1. The browser parses the HTML first to understand all the components it needs to compile in order to render the page.
2. The browser looks through the HTML document to see if external CSS files have been linked using the `<link>` tags or if external JavaScript files have been linked using the `<script>` tags.
3. When the browser finds those elements, it sends requests to the server to fetch the referenced files.
4. Upon receipt of the files from the server, the browser parses the CSS and stores the values in memory along with the HTML values, then parses, compiles, and executes the JavaScript.

The end result is a rendered webpage.

## How to find images to add to a Website

There are many sites that offer free images to add to your website. One well-known website is the [Google Images](https://www.google.com/imghp). Another popular site is [Shutterstock](https://www.shutterstock.com/). These sites allow you to search for the image you desire.

## Creating a String vs a Number in JavaScript?

To assign a string to a variable in JavaScript, you simply need to **double-quote** or **single-quote** the value. To assign a number to a variable, you would do the opposite (no quotes) but only with numerical values. Example:

```javascript
const thisIsAString = “myString”
let thisIsANumber = 10
```

## JavaScript variables and why they are important

Variables in JavaScript (and pretty much all other languages) serve as named containers that store values. This capability of variables allows code/programs to store dynamic values and retrieve them when needed.

## HTML attributes

An HTML attribute refers to the extra information that can be declared/added inside of elements. They can either be optional or required, depending on the type of element. A common example of an HTML attribute is the `class` attribute, which is generally used by CSS or JavaScript to style an element or group of elements. Example:

```html
<div class="my-class">My Class</div>
```

## Anatomy of an HTML element

An HTML element consists of the following:

1. **opening tag**: consists of the two angle brackets `<>`, encasing the element’s name `<div>`.
1. **element name**: name of the element i.e., `div`, `img`, `p`, `body`, etc., encapsulated by either the opening or closing bracket.
1. **attributes**: the extra (or required) information allowable for the specified element.
1. **content**: the content between the opening and closing tags. Usually text, but can be other forms of data as well.
1. **closing tag**: similar to the opening tag but contains a forward slash after the first angle bracket and before the element name `</div>`. This tag signifies the end of the element.

## The difference between `<article>` and `<section>` element tags

An `<article>` element tag is used for a block of content that remains relevant regardless of all other elements. A `<section>` element tag on the other hand, is used to group functionally similar sections of a webpage.

## Elements of a “typical” website

A typical webpage generally contains the following elements:

* `<html>` element: the root of all elements
* `<head>` element: contains metadata for the site
* `<body>` element: contains the visible content of the page
* `<header>`, `<nav>`, `<main>`, `<footer>`: these elements are usually found within the `<body>` element and are know as `semantic elements`. They help organize the structure of the page.

## How metadata influences Search Engine Optimization

A website’s metadata provides information to the browser as well as search engines. The more information provided by the metadata, the more information a search engine can cache and present to searchers, subsequently optimizing the searches for the presented content. Also, search engines use metadata to rank webpages when searched (effects whether your content appears on the first page of searches or not)

## The `<meta>` HTML Tag and Metadata

The `<meta>` tag is the orthodox way of adding metadata to a webpage. The `<meta>` element can be used to specify the encoding, the description, the author of a website, and much more.

## How to start to design a Website

1. What is the first step to designing a Website?
    * Deciding what you want your website to accomplish.
2. What is the most important question to answer when designing a Website?
    * What is the primary purpose or goal of the website?

## Semantics

1. Why should you use an `<h1>` element over a `<span>` element to display a top level heading?
    * Because an `<h1>` element is specifically designed for a top level heading. A `<span>` element does not inherently styled an element, and is generally used by CSS to style a specific portion of text.
2. What are the benefits of using semantic tags in our HTML?
    * Semantic tags in HTML help structure the web page (for the viewer as well as the browser), allow assistive technology to work with the site, and allow SEO to understand the context and content of the site.

## What is JavaScript?

1. Describe 2 things that require JavaScript in the Browser?
    * Two things that require JavaScript in the Browser are: form validation and dynamic content manipulation.
2. How can you add JavaScript to an HTML document?
    * JavaScript can be added to an HTML inside the document within a script element or in a separate javascript file linked inside the `<src>` of a script element.

## Things I want to know more about

I want to know more about the `<svg>` element.
