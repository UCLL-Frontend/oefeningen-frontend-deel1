# Style your documents using CSS

## Link to Exercises Week 2
[Link to exercises week 2](https://github.com/UCLL-Frontend/oefeningen-frontend-deel1/blob/main/week-02-create-the-homepage-of-your-static-website.md)

## Description

In the last exercise, you created your first HTML document (homepage). The goal of this exercise is now to style that page using CSS, working for a small screen (width 400 pixels). In the next lessons, you will learn how to move blocks around so that you make the best use of wide screen space.

During the course, you learned about external CSS files, embedded CSS, inline CSS, selectors… Time to turn this into practice. Open your homepage and resize the browser screen.

## Specifics

- Start by reviewing the HTML document created in the previous exercise. Understand its structure, elements, and content.
- Create in your project directory a folder "CSS". Create a new external CSS file with a .css extension in that directory. You can name it something like styles.css. This file will contain the styles for your HTML document.
- In the HTML document's `<head>` section, link to the external CSS file using the `<link>` element.
- In your external CSS file (styles.css), apply styles to various elements of the HTML document. We give some suggestions:
  - Play with colors (background-color, color of text). For example:
    - Change color of all text to #333.
    - Create colorset for "dark mode" (dark background-color and text in color with a lot of contrast).
    - Give footer and header contrasting background-color.
  - Choose a nice font-family. Do not hesitate to choose a different one for headings and normal text.
    - Change font-family from serif to non-serif.
    - Try some [Web Safe Fonts](https://blog.hubspot.com/website/web-safe-html-css-fonts).
  - Resize text. Choose an appropriate line-height.
  - Play with selectors. For example:
    - Give the links in the navigation a different color than the links elsewhere in the text.
    - Show the first list-item in another color than the other list-items.
    - Give the headers a font-family different from the rest of the text.
  - Play with width in CSS. Example: resize figures to full browser width.
  - Play with padding and margin: use this to visually separate consecutive blocks.
- In the `<head>` of your HTML document, you can also include embedded CSS using the `<style>` element to apply specific styles to elements within that document.
- Practice inline style by using styles directly on individual HTML elements using the style attribute.
- Open your HTML document in a web browser and test the styles. Resize the browser window to see how the responsive styles for small screens work.
- Feel free to experiment with different styles, colors, and layouts to achieve the desired look and feel for your HTML document.
- It's good practice to add comments in your CSS code to explain the purpose of different style rules and provide context for your styling decisions.
- ??? Color contrast analyzer can be introduced here.
- Test using [HTML5 Validator](https://html5.validator.nu/) if each HTML page is valid according to the current web standard HTML5.
- Test using [CSS Validator](https://jigsaw.w3.org/css-validator/) if your CSS file is valid according to the web standard CSS3.

## How to Submit

Deliver the assignment on the webserver. It must be available on the class list under the title "site". The URL should be as [https://r0934094.webontwerp.ucll.be/site](https://r0934094.webontwerp.ucll.be/site).

## Deadline

This exercise is considered as exercise on lesson 2. You must deliver it as part of "Tussentijdse opdracht" with deadline 12/10.

## Self Assessment

Check your submission yourself:

### Technique

- The HTML is valid (check on [HTML5 Validator](https://html5.validator.nu/) or [W3C Validator](https://validator.w3.org/)).
- The CSS code is valid (check on [CSS Validator](https://jigsaw.w3.org/css-validator/)).
- Your website has an external style sheet, in the folder CSS.
- You have used most types of CSS selectors: HTML elements, id, class, child selector, combination of all.
- You have used the properties color, background-color, font-family, line-height, font-size, and more.
- At least one element is limited in width (including max-width).
- You have used the properties margin and padding.
- Padding and margin are not applied cumulatively (where not necessary/where possible). Example: both body and article have padding-left so that they add up to a wide padding-left.
- You use margin and padding to create white space, not <br>.
- CSS code is repeated as little as possible (DRY).

### Layout

- When you resize the browser screen to 400px, there is no horizontal scroll bar.
- The page has a good vertical alignment.
- The colors are well combined.
- The different levels of headings are visibly distinguished.
- The line-height corresponds to the chosen font-family and font-size.
- The naming of selectors is properly chosen.
