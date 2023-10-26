# Evaluation Criteria

Front End Development, October 2023

The requirements of the assignment when developing your website can be found at [Toledo > Assignments & Tests > Assignment HTML and CSS](https://github.com/UCLL-Frontend/oefeningen-frontend-deel1/blob/main/assignment-module-1.md) (including scope, content, objectives, ...). During the lessons you got a new piece to the assignment each time (other files in [this repo](https://github.com/UCLL-Frontend/oefeningen-frontend-deel1)) with some criteria each time that you could test yourself. This text is a summary of the _technical_ criteria you were already given, supplemented with some details, pitfalls and possible solutions.

Reflect again on the elaboration of the website as it nears completion. What did you already do well? What could be done better?

<section>

### 1\. Validation

* Every HTML file has an HTML5 declaration.
    * first line file must be: `<!DOCTYPE html>``
* Every HTML file validates according to the HTML5 doctype at [https://validator.w3.org/](https://validator.w3.org/) or [https://html5.validator.nu/](https://html5.validator.nu/).
    * Read the error messages (errors, indicated in red) carefully. They indicate what error you made and often also a hint to solve them.
    * Using Google map causes problems: see [documentation 'responsive Google Map'](https://www.labnol.org/internet/embed-responsive-google-maps/28333/) for a solution.
    * when using `iframe` for map you have to remove frameborder attribute completely to validate, a.o. for Google Map, ...
    * images:
        * attribute `alt=""` do not forget to add
        * Empty images (with `src=""`) do not validate
        * image in a list: either `img` element surrounded by `li`, or `img` placed outside the list
    * Place `header` in `head` instead of `body`.
    * use non-existent elements such as `p1`, ...
    * warnings (yellow) are allowed, try to keep them to a minimum
* The CSS file validates at [https://jigsaw.w3.org/css-validator/](https://jigsaw.w3.org/css-validator/).
    * Read the error messages carefully. These indicate what error you made and often a hint on how to fix them.
    * Pay attention to unnecessary or not allowed spaces e.g. when using units (`margin`:`**1.2rem**` and not `margin:**1.2 rem**`);
    * use correct properties and values, e.g. `flex:right` does not exist but `display:flex` and `align-content:flex-end` do;

</section>

<section>

### 2\. File structure

* All (S)CSS files are grouped in one folder (possibly with subfolders)
    * you use SCSS to generate CSS
    * this results in one _own_ CSS file, so no separate file per html page;
* Images are grouped in the "img", "images" or similar folder.
* Links to CSS and images from the HTML file are relative.
    * So e.g. not: file:///Users/krmel/web1/img/logo.png but rather img/logo.png;

</section>

<section>

### 3\. HTML - Document Structure

* You use semantic HTML (including header, nav, main, footer, article, section, aside, address, ...) _in every page_ (including the contact page and portfolio, if you have them).  
    Common mistakes:
    * you don't use a `main` element
    * You do not use or barely use the elements `article` and `section`, or too much.
    * you improperly use `div` (instead of `article` or `section`) i.e. no use of `div` when other elements are applicable, see [html5doctor sectioning flowchart](http://html5doctor.com/downloads/h5d-sectioning-flowchart.png)
* Header contains `h1` with site name and `nav`.  
    Common errors:
    * `header` contains `ul` with links in `header` without `nav` element
    * `header` contains only 1 of both, this is possible if `h1` is in the `header`.
    * Use `nav` for sure
* Navigation is a list (`ul`).
    * Listing only links is not OK because of accessibility.
* Every sectioning element has a header (`h2`, `h3`, ...).
    * follow hierarchy: h1=title/topic whole website, h2=page title, h3=subtitle of the page, ...
    * do not skip levels e.g. from `h1` to `h4`
    * if not every sectioning element has a header, this gives a 'warning' no error. Check if you use sufficient and clear headers in connection with 'usability' and 'accessibility'.
* `section` and `article` are used correctly.
    * Both group content that belongs together.
    * `article` stands alone and you would include in a table of contents, can also include a `header` and a `footer` to indicate when and by whom written
    * Use `div` only to group content for style purposes and not for the sake of content consistency
* Structure elements are not used for layout
    * if you 'turn off' the styles, e.g. via Web Developer Toolbar - CSS - disable all styles, then the structure should be apparent from the page.
    * tables
        * Do not use tables for layout
        * Not all content is suitable for tables, e.g. if there are no recurring titles.
        * if using a table in an allowed context, ensure maximum accessibility ([Web Accessibility Tutorials - tables concepts](https://www.w3.org/WAI/tutorials/tables/))
        * Ask yourself if it is an option to use a list instead of a table

</section>

<section>

### 4\. HTML - Separation of content and structure.

* No `br` is used to create whitespace.
    * Use `margin` and `padding`.
* Text is divided into paragraphs.
    * Is sometimes related to too much use `br` and too little `p`
    * make sure there is enough text and therefore enough `p`

</section>

<section>

### 5\. HTML - Hyperlinks

* Links within the site are relative, not absolute.
* All links work, including on the web server.  
    Common errors.
    * naming inconsistent between link and actual file (overOns.html vs. overons.html)
    * wrong path
    * your laptop is not case sensitive, but the web server is.

</section>

<section>

### 6\. HTML - Images

* If necessary, images are placed in the figure element.
* The loading speed is small:
    * images are stored in the maximum size that they will be used on the website (for the mobile version as well as desktop version), e.g.. Facebook logo 600px x 400px too large.
    * Images are sufficiently compressed.
* A meaningful alt attribute is used with the images.
    * alt="" for purely decorative photos/images
    * alt="image of number of registrations course Applied Computer Science AJ 2020-2021 (UCLL)" ==> omit 'image of'
    * alt="logo company" ==> alt="Red Cross, helping help"
* Links to CSS and images from the HTML file are relative.
    * so e.g. not: file:///Users/krmel/web1/img/logo.png but rather img/logo.png;

</section>

<section>

### 7\. Layout

* Custom color use.
    * use a [proper notation](http://hslpicker.com/), see e.g. [http://hslpicker.com/](https://hslpicker.com/): not the color name like 'white', but e.g.. #000 (hexadecimal), or rgb(255, 255, 255) (rgb) or hsl(360, 100%, 100%), and rgba(255, 255, 255, 1) or hsla(360, 100%, 100%, 1) (hsla) to use the alpha channel for 'opacity' effect
    * Limit the number of colors used, e.g. compose your color palette with [Adobe color wheel](https://color.adobe.com/nl/) by using the wheel, using an existing theme or compose a color palette based on your own photo/logo, or specific color
* Custom fonts and sizes and line-height.
    * Choose some fonts that go well together
    * get inspiration from [Google Fonts](https://fonts.google.com/), and [FontSquirrel](https://www.fontsquirrel.com/)
    * always end `font-family` with serif or non-serif;
* Sufficient contrast, be careful with text on dark surfaces or images, use the [Colour Contrast Analyzer](https://developer.paciellogroup.com/resources/contrastanalyser/).
* Correct alligning: be careful with centering (better too little than too much)! Provide clear horizontal and vertical lines
* Make sure content that belongs together is also visually displayed as a whole that belongs together (forms together with previous items [CRAP](http://frontend.webontwerp.ucll.be/CSS_CRAP/) principle).
* Images: [edit](https://cloudinary.com/documentation/image_transformations) your images so that they are not too large in pixels nor in kB.

</section>

<section>

### 8\. CSS - SCSS

* You use SCSS to generate CSS.
* Your SCSS files are on the server in the same folder as your CSS file(s).
* SCSS is made up of components that have a logical structure.
* The associated CSS is in partials or subfiles (e.g., `_header.scss`) that are organized into folders (directories).
* You use nesting.
* You use variables.

</section>

<section>

### 9\. CSS - Positioning.

* You use the right technique in the right place.
* `Flex` is used correctly.
    * 1D (one-dimensional), so use for navigation, but e.g. also for `footer`
    * Do not use (earlier) for full page layout
* `Grid` is used correctly.
    * 2D (two dimensional), so use for full page layout (main components) and 1 level down.
    * Use the possibilities of grid, work where possible with gap instead of margin/padding
* Text blocks have no fixed height.
* Position:absolute is used sparingly or not at all.
* `Position:absolute` is used in combination with position:relative of a parent element (that way it is positioned absolutely relative to that parent).
* You use a normalize.css (optional).
    * for example [normalize.css](https://necolas.github.io/normalize.css/)
    * specificity: insert the normalize.css first, only then own styles!

</section>

<section>

### 10\. CSS - Selectors

* CSS code is repeated as little as possible (DRY).
    * E.g., by defining default styles for `body`, by grouping selectors, ...
    * CSS rules are made as general as possible, e.g. `padding` for the enclosing div instead of `margin` for each individual `p`.
* Good readable naming of id and class attributes.
    * Use `id` and `class` with moderation.
    * naming best refers to the intended effect of the class, (e.g., `class="right"` for all images to appear on the right), so not `class="photo1"`
* If there is a group of elements that have the same CSS properties, a group selector is used (e.g. `h1,h2`{ ...}).

</section>

<section>

### 11\. RWD

* In the HTML file, the head contains the element `<meta name="viewport" content="width=device-width, initial-scale=1">.
* The number of breakpoints is limited.
    * Work out 3 to 5 breakpoints, it does not have to be 10.
* The breakpoints are well chosen.
* Preferably work mobile first, so `@media` ... and (`**min-width**`:...)
* Test in Firefox with Developer toolbar>Resize>View responsive layouts (or similar tools) gives good results.
* Test with own smartphone/tablet gives good results.
* If necessary, content disappears. Not too much content disappears.
* Widths of blocks are (usually) relatively defined (if necessary).
    * use `rem`, `%` or `fr` (grid) for widths of sections, articles, paragraphs;
    * for margins and paddings you can also use relative units e.g. values expressed in `rem` (or in %);
* widths of images are defined relatively (if needed).
    * e.g. set the width of your image relative to the container with `max-width:100%;` and/or `width:100%;` and ensure proportional images with `height:auto;`.
* After saving in the correct dimensions, the images were compressed and optimized, e.g. via [Cloudinary](https://cloudinary.com/users/login)

</section>

<section>

### 12\. Accessibility

* The layout is good in Edge, Firefox, Safari and Chrome.
* Fontsize is relatively defined.
    * Do not use `cm`, `mm` or `pt`, but preferably no `px` either.
* Your website passes at least the 15 critria of the [Quickscan by Anysurfer](https://toegankelijkheidsmonitor.be/2020.html) (under the heading "How did websites score?"), or better yet the [checklist by WebAIM](https://www.anysurfer.be/nl/documentatie/artikels/detail/webaims-wcag-2-checklist). You can also use the [Wave Browser Extension](https://wave.webaim.org/) to test your Web site. 

</section>

<section>

### 13\. Usability

* Each page has a specific `title`, `h1`, and `h2`.
    * `title`: reference to subject AND/Or specific page missing
    * `h1`: displays subject website
    * `h2`: displays page title, link to current menu item
* Load speed is fine.
* Optimal screen utilization at all resolutions (take care of media queries that place content blocks differently according to screen width, among other things)
* Clear navigation
    * The current page is highlighted in the menu. Add e.g. a class="current" to indicate the current page and style accordingly in CSS;
    * Menu items: clear naming and well-chosen order of menu items
* Clear links:
    * clear link description (i.e., not "click here")
    * Clearly distinguishable design
* Sound content:
    * relevant content
    * writing for the web: Keep It Short and Simple (KISS), think about your target audience, ...
    * scannable display: sufficient paragraphs, working with lists or highlighting words via `strong` and `em`, max. 60-70 characters on a reading line, ...
    * most important at the top
* Make use of conventions: logo, ID, navigation, ...
* Ensure consistency throughout your website

</section>

<section>

### 14\. Form

* Is meaningful and relevant to target audience, takes into account aspects of `usability'
* Has sufficient complexity: at least 3 different `input` types, in addition to type "submit"
* Has custom layout (via css) with special attention to `mobile` display
* Client-side validation
    * Use attribute `required`.
    * Use correct `input type`
* Is accessible, see [WAI Tutorial - forms](https://www.w3.org/WAI/tutorials/forms/), and also:
    * [labels and form fields are connected](https://www.anysurfer.be/nl/documentatie/artikels/detail/verbind-labels-met-formuliervelden)
    * required fields are announced within label, and attribute `required` is used

</section>

<section>

### 15\. And further

* Consistent file names by convention
    * No spaces or special characters in file names:
        * not 'about us.html', but overOns.html, over_us.html or over-us.html
        * not q&a.html, but qAndA.html, q_and_a.html or q-and-a.html
    * always lowercase for files: logo.png and not Logo.png or logo.PNG or DSC1234.png, ...
    * same for folders: folder images and not Images
    * index.html (not home.html, Index.html, index Laundry.html, ...)
* Web page is performant in terms of speed, accessibility, ...: [Lighthouse on Google Chrome](https://developers.google.com/web/tools/lighthouse/) (Inspect Element > Audit) gives immediate information about the entire website, also accessibiltiy

</section>