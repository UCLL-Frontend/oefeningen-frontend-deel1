# Style your documents using CSS – Box Model

## Link to Exercises "Create the Home Page"
[Link to Exercises Create the Home Page](https://github.com/UCLL-Frontend/oefeningen-frontend-deel1/blob/main/week-02-create-the-homepage-of-your-static-website.md)

## Description

The result of the previous exercise is rather good. But aren't the titles very short on the next paragraph? And isn't the image a bit large? In this exercise, we are going to improve it, again for a small window.

Open your homepage and resize the browser screen to 600px. Also in this exercise, we limit ourselves to a small-screen layout.

## Specifics

- Add CSS rules in your CSS file (no inline or embedded styles).
- Play with padding and margin. Use the developer tool to discuss the result.
- Use padding and margin to visually separate consecutive blocks (e.g. h2 and following p). Try both.
- Add a border and background color to the navigation items. Add padding such that they don’t stick to the edge.
- Play with width in CSS. Examples:
  - Resize figures to full browser width, to 50% of the browser width, 600px … Resize the browser screen and discuss the result.
  - Put the resized image in the center of the containing block.
- Play with the width of the main content (header + main + footer).
  - Limit the size of the main content to 70% of browser width. Give the outer margin a contrasting color. Make sure the container is in the center of the screen.
  - Do the same, but set the width to 600px (fixed width). Resize the browser screen and see what happens.
  - Make a combination of both: set the width to 90% and max-width to 600px.
  - Try another view: Make the header and footer as wide as the screen and limit the element main to 70%. Write as few CSS as possible. You can do this exercise on another HTML page if you want.
- Create a nice vertical navigation for a small screen.
  - Eliminate the bullets of the list with list-style-type: none.
  - Give the current link (the page where you are right now) a ‘reversed effect’: dark letter on a light background.
  - Create a hover-effect [hover](https://developer.mozilla.org/en-US/docs/Web/CSS/:hover).
  - Maybe you can try a smooth transition [transition](https://developer.mozilla.org/en-US/docs/Web/CSS/transition).

Open your HTML document in a web browser and test the styles. Resize the browser window to see how the responsive styles for small screens work.

Feel free to experiment with different styles, colors, and layouts to achieve the desired look and feel for your HTML document.

Test using [HTML5 Validator](https://html5.validator.nu/) if each HTML page is valid according to the current web standard HTML5.

Test using [CSS Validator](https://jigsaw.w3.org/css-validator/) if your CSS file is valid according to the web standard CSS3.

## How to Submit

Deliver the assignment on the webserver. It must be available on the class list under the title “site”. The URL should be as [https://r0934094.webontwerp.ucll.be/site](https://r0934094.webontwerp.ucll.be/site).

## Deadline

This exercise is considered as exercise on the lessons of CSS: Box Model. You must deliver it as part of “Tussentijdse opdracht” with a deadline of 12/10.

## Self Assessment

Check your submission yourself:

### General
- Your webpage is available via [our webserver](https://webontwerp.ucll.be/Ti-Front-end/reeksen/reeksoverzicht.html). Use FileZilla to transfer the *all* files (*including directories with css, images, ...*) from your device to the webserver ([manual on this link](https://frontend.webontwerp.ucll.be/HTML_basispg/#FTP-(File-Transfer-Protocol))). 

### Technique

- The HTML is valid (check on [HTML5 Validator](https://html5.validator.nu/) or [W3C Validator](https://validator.w3.org/)).
- The CSS code is valid (check on [CSS Validator](https://jigsaw.w3.org/css-validator/)).
- At least one element is limited in width (including max-width).
- You have used the properties margin and padding.
- Padding and margin are not applied cumulatively (where not necessary/where possible). Example: both body and article have padding-left so that they add up to a wide padding-left.
- You use margin and padding to create white space, not `<br>`.
- CSS code is repeated as little as possible (DRY).

### Layout

- When you resize the browser screen to 400px, there is no horizontal scroll bar.
- The page has a good vertical alignment.
- The colors are well combined.
- The different levels of headings are visibly distinguished.
- The naming of selectors is properly chosen.
