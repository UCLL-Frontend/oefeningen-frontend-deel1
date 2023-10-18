# Expand your static website and layout your page using grid and flexbox

## Description

Expand your static website with three extra HTML documents (= total of at least four documents plus site specification). Form the layout of these pages using at least flexbox and CSS grid once. Keep the RWD (Responsive Web Design) principles in mind.

## Specifics

- Start by creating three new HTML files, each representing a new page on your website. For example, you can create `about.html`, `services.html`, and `contact.html`.
- Use the correct HTML5 document structure, including the `<!DOCTYPE html>` declaration, `<html>`, `<head>`, and `<body>` elements.
- At this point, it can be usefull to add a CSS reset class (e.g. [normalize.css](http://necolas.github.io/normalize.css/)).
- In one of the new HTML files (e.g., `about.html`), create a layout using Flexbox. For example, create a section with multiple elements that are laid out horizontally (wide screen) or vertically (small screen) using Flexbox properties like `display: flex`, `flex-direction`, `justify-content`, and `align-items`.
-   In your `style.css`, apply Flexbox styles to the elements within the flex-container.
  - Use media queries to make the layout responsive. Work mobile-first.
- In the other new HTML file (e.g., `services.html`), create a layout using CSS Grid. For example, create a grid container with multiple grid items.
  - In your `style.css`, apply CSS Grid styles to the elements within the grid-container.
  - Use media queries to make the layout responsive.
- Ensure that your navigation menu, which you have already created in your `index.html`, includes links to the newly added pages (`about.html` and `services.html`). Remember that the fifth link must link to your site specification. 
- Make sure to use media queries to make your layout responsive, including navigation, images, white spaces, etc. Work mobile-first.
- Test the validity of each of your HTML pages using an online validator, such as [https://html5.validator.nu/](https://html5.validator.nu/). Ensure that there are no errors or warnings in the validation reports.
- Test using [CSS Validator](https://jigsaw.w3.org/css-validator/) if your CSS file is valid according to the web standard CSS3.

## How to Submit

Deliver the assignment on the webserver. It must be available on [the class list](https://webontwerp.ucll.be/Ti-Front-end/reeksen/reeksoverzicht.html) under the title “site”. The URL should be as [https://r0934094.webontwerp.ucll.be/site](https://r0934094.webontwerp.ucll.be/site).

## Deadline

This exercise is considered as exercise on the lessons of CSS: Flexbox, grid, and RWD. You must deliver it as part of “Opdracht HTML en CSS”, with a deadline of 15/11/23.

## Self Assessment

Check your submission yourself:

### Technique

- The HTML is valid (check all pages on [https://html5.validator.nu/](https://html5.validator.nu/) or [https://validator.w3.org/](https://validator.w3.org/)).
- The CSS code is valid (check on [https://jigsaw.w3.org/css-validator/](https://jigsaw.w3.org/css-validator/)).
- CSS code is repeated as little as possible (DRY) (this also applies to media queries).
- Images are grouped in a folder “img” or “images”.
- The download size is small: images are stored in the maximum size that they are used on the website and they are compressed optimally.
- You use flex at least once, for one-dimensional layout, only where relevant.
- You use grid at least once, for two-dimensional layout, only where relevant.
- You do not mix positioning techniques as grid and layout for the same container.
- Width and height are relatively defined (when necessary).

### General

- When you resize the browser screen as small as possible, there is no horizontal scroll bar.
- The page has a good vertical and horizontal alignment.
- The naming of selectors is properly chosen.
- Your website is responsive. The breakpoints are well chosen.
