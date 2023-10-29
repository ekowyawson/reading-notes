# Class 05: Images, Color, Text

![Image of CSS and HTML Logos](css-image2.png)

Images, color, and text are most of what websites comprise of. They are, quite literally, the reason people visit a website. For this purpose, it is very important to pay close attention to these elements when designing and building a website.

## HTML Media

### What is a real world use case for the `alt` attribute being used in a website?

Two real world use cases for the `alt` attribute of the `<img>` element are:

* To display a text description of the image if the image fails to load or loads slowly
* To allow screen readers to read an image description to visually impaired people

### How can you improve accessibility of images in an HTML document?

You can improve accessibility of images in an HTML document by utilizing captions and `alt` attributes, along with thoughtful and distinct text for both.

### Provide an example of when the figure element would be useful in an HTML document

The `<figure>` element allows you to place an image and caption (using the `<figcaption>` element) within a container. This is useful when you have numerous images on a page but want to code for accessibility as well, allowing screen readers an ability to succintly read each caption.

### Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community

A GIF image is like a flipbook: It's made up of a series of pictures, and when you look at them one after the other, it looks like a short animation.

An SVG image, on the other hand, is more like a magical picture. It's made using instructions, kind of like a recipe for drawing. Instead of having lots of pictures like in a GIF, an SVG tells the computer how to draw shapes and lines to create an image.

### What image type would you use to display a screenshot on your website and why?

To clearly display a screenshot on your website, you would want to use a **lossless** format (an image compression format that doesn't lose bits of the original image). Lossless image format examples are **PNG** and **WebP**.

## CSS

### Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge

Imagine that an HTML element on a webpage is like a picture frame. The foreground color is the color of the picture or artwork inside the frame (what you see when you look at the picture). If the picture is of a blue ocean, the color of the ocean is the foreground color because it is what grabs your attention.

On the other hand, the background color is like the color of the wall behind the picture frame. It's what surrounds the picture, and it can be any color you choose. For example, you might hang the picture on a yellow wall (the background color is now yellow), which sets the mood and context for the picture.

### Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

You can use CSS colors to add character and style to a colorless blog website by carefully selecting a color scheme and applying it to various elements. First, you would choose a color palette that either compliments or contrasts. Using the colors from the color palette, you could then use accents for the header and navigation. Next, you would use a soft or muted color for the background, that complements the whole scheme. Finally, you would carefully select colors for links, borders and other elements that make those elements pop.

### What should you consider when choosing fonts for an HTML document?

When choosing fonts for an HTML document, it is important to consider what fonts are available for all devices. In order to ensure your font choice is available for all devices, you should opt to use **web safe fonts** (a number of fonts that are generally available across all systems).

### What do font-size, font-weight, and font-style do to HTML text elements?

* **font-size**: determines the size of the text
* **font-weight**: determines the thickness/boldness of the text
* **font-style**: determines the style of the text; for example: *italic* or *oblique*

### Describe two ways you could add spacing around the characters displayed in an `<h1>` element

Two ways you could add spacing to around characters in an `<h1>` element are by using `letter-spacing` and `word-spacing` declarations.

## Things I want to know more about

I would like to practice more using the `<svg>` and `<canvas>` elements to draw vector graphics on my webpage.
