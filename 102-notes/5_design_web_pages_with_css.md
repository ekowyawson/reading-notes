# Design Web Pages With CSS

![Alt text](../images/css_image.png)

Once upon a time in the world of web development, there was a talented young programmer named Nosway. He had conquered the world of HTML and JavaScript, but there was one formidable beast that still eluded him: **Cascading Style Sheets** (CSS).

Nosway had always found CSS to be a mysterious, yet, touchy beast. It was like an artist's palette with endless colors, fonts, and layout possibilities, and it often felt as if CSS had a mind of its own. One gloomy evening, determined to conquer the beast, Nosway set out to tackle a particularly tricky project: redesigning a professional blog.

Guess what? We are Nosway, and Nosway is us. Let us dive neck deep into CSS.

## What is CSS

CSS stands for *Cascading Style Sheets*. It is used to style web pages. In the early days of the internet (early 1990's), web pages were primarily made up of plain old HTML, which mainly focused on the page structure. Web developers at the time had to rely on HTML attributes and elements to control the presentation of web pages. This led to inconsistencies and maintenance difficulties. Those of you who were aware at that time will remember.

The need for a separate technology to handle the styling and layout of web pages became increasingly apparent. In 1994, **HÃ¥kon Wium Lie** proposed the idea of CSS to the *World Wide Web Consortium* (**W3C**). W3C accepted HÃ¥kon Wium Lie's proposal, adopted, and published the first CSS specification *CSS1* in 1996.

Today, CSS has evolved so much that it has now has multiple dedicated frameworks.

## What is the purpose of CSS?

As discussed previously in this blog, CSS is primarily used to style webpages (to make it look pretty... or professional.)

## What are the three ways to insert CSS into your project?

The three ways to insert CSS into your web project are: 1) external; 2) internal; 3) inline:

1. **External CSS**: To add an external CSS, you would create a separate file, with a *.css* extension, within your folder structure. You would then link that css file to your *html* file by using `<link>` tags inside the `<head>` element.
2. **Internal CSS**: To add internal CSS to your project, you would write the CSS code directly inside the html file using `<style>` tags inside the `<header>` element.
3. **Inline CSS**: Inline CSS, as the name implies, is added directly to the specific line, or tag, that you are currently writing. The CSS code would be placed inside the element's beginning tag as a `style` attribute.

## An example of a CSS rule that would give all `<p>` elements red text

```css
p {
    color: red;
}
```

## Resources

1. [History of CSS](https://www.bu.edu/lernet/artemis/years/2020/projects/FinalPresentations/HTML/historyofcss.html#:~:text=1994%2D%20H%C3%83%C2%A5kon%20Wium,separate%20documents%20known%20as%20modules)
2. ChatGPT (*used to requisition a small subset of answers*)
