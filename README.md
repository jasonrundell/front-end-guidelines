# Coding Guidelines

# Table of contents

- [Purpose](#purpose)
- [Contributing](#contributing)
- [Browser and device support](#browser-and-device-support)
  * [Minimum browser support](#minimum-browser-support)
  * [Minimum device support](#minimum-device-support)
- [Testing](#testing)
  * [Browser and device testing](#browser-and-device-testing)
    + [Chrome testing on Mac/iOS/Windows/Android](#chrome-testing-on-mac-ios-windows-android)
    + [Edge testing on Mac/iOS/Windows/Android](#edge-testing-on-mac-ios-windows-android)
    + [Firefox testing on Mac/iOS/Windows/Android](#firefox-testing-on-mac-ios-windows-android)
    + [IE 11 testing on a Mac](#ie-11-testing-on-a-mac)
    + [iOS device testing on a Mac](#ios-device-testing-on-a-mac)
    + [Safari testing on a Mac/iOS](#safari-testing-on-a-mac-ios)
- [Code quality](#code-quality)
  * [General Principals](#general-principals)
  * [General Methodologies](#general-methodologies)
    + ["Mobile-first" development](#-mobile-first--development)
      - [Hierarchy of audience](#hierarchy-of-audience)
      - [Gesture-first mind-set](#gesture-first-mind-set)
- [HTML](#html)
  * [HTML principles](#html-principles)
  * [HTML tools](#html-tools)
  * [HTML syntax](#html-syntax)
- [CSS](#css)
  * [CSS methodology](#css-methodology)
  * [CSS syntax](#css-syntax)
  * [CSS tools](#css-tools)
  * [CSS frameworks](#css-frameworks)
- [SASS](#sass)
  * [SASS methodologies](#sass-methodologies)
    + [File Naming](#file-naming)
  * [SASS syntax](#sass-syntax)
- [JavaScript](#javascript)
  * [JavaScript principals](#javascript-principals)
  * [Types](#types)
  * [References](#references)
  * [Objects](#objects)
  * [Arrays](#arrays)
  * [Destructuring](#destructuring)
  * [Strings](#strings)
  * [Functions](#functions)
  * [Arrow Functions](#arrow-functions)
  * [Classes & Constructors](#classes---constructors)
  * [Modules](#modules)
  * [Iterators and Generators](#iterators-and-generators)
  * [Properties](#properties)
  * [Variables](#variables)
  * [Hoisting](#hoisting)
  * [Comparison Operators & Equality](#comparison-operators---equality)
  * [Blocks](#blocks)
  * [Control Statements](#control-statements)
  * [Comments](#comments)
  * [Whitespace](#whitespace)
  * [Commas](#commas)
  * [Semicolons](#semicolons)
  * [Type Casting & Coercion](#type-casting---coercion)
  * [Naming Conventions](#naming-conventions)
  * [Accessors](#accessors)
  * [Events](#events)
  * [jQuery](#jquery)
  * [Standard Library](#standard-library)
  * [Testing](#testing-1)
  * [JavaScript methodology](#javascript-methodology)
  * [JavaScript tools](#javascript-tools)
  * [JavaScript syntax](#javascript-syntax)
- [React](#react)
  * [Alignment](#alignment)
  * [Quotes](#quotes)
  * [Spacing](#spacing)
  * [Props](#props)
  * [Refs](#refs)
  * [Parentheses](#parentheses)
  * [Tags](#tags)
  * [Methods](#methods)
  * [`isMounted`](#-ismounted-)
  * [CSS-in-JS](#css-in-js)
- [Media](#media)
  * [Icons](#icons)
  * [Tools](#tools)
- [Typography](#typography)
  * [Fonts](#fonts)
- [Performance](#performance)
- [Accessibility](#accessibility)
  * [Tools](#tools-1)
- [Tooling](#tooling)
  * [ESLint](#eslint)
- [Version control](#version-control)
  * [Git](#git)
    + [Commits](#commits)
    + [Branching](#branching)
    + [Merging](#merging)
  * [GitHub](#github)
    + [Pull Requests "PR"](#pull-requests--pr-)
    + [Code reviews](#code-reviews)
      - [Reviewer](#reviewer)
      - [Reviewee](#reviewee)
- [Localization](#localization)
- [Deployment/Integration](#deployment-integration)
- [Documentation](#documentation)
  * [In-line code comments](#in-line-code-comments)
  * [README documentation](#readme-documentation)
- [Kudos](#kudos)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>

# Purpose

This documentation lives to establish the coding guidelines for a Front End development team.

> **"It's to help us deliver high quality content that works better, reaches more
> people - not only in today's browsers & devices, but in tomorrows."**
>
> _[yellowshoe.com.au/standards/](https://yellowshoe.com.au/standards/)_

> **A coding styleguide (note, not a visual styleguide) is a valuable tool for
> teams who:**
>
> - **build and maintain products for a reasonable length of time;**
> - **have developers of differing abilities and specialties;**
> - **have a number of different developers working on a product at any given
>   time;**
> - **on-board new staff regularly;**
> - **have a number of codebases that developers dip in and out of**
>
> _[Harry Roberts](http://csswizardry.com/) states it very well in 
> [CSS Guidelines](http://cssguidelin.es/#the-importance-of-a-styleguide)_

> **"Part of being a good steward to a successful project is realizing that writing code for yourself is a Bad Idea™. If thousands of people are using your code, then write your code for maximum clarity, not your personal preference of how to get clever within the spec."**
>
> _Idan Gazit_

**[⬆ Back to top](#table-of-contents)**

# Contributing

For additions or contributions to these code guidelines,
[please open an issue](https://github.com/jasonrundell/coding-guidelines/issues).

**[⬆ Back to top](#table-of-contents)**

# Browser and device support

## Minimum browser support

- IE 11 version 11.x
- Safari 11.1
- Edge latest -2
- Firefox latest -2
- Chrome latest -2

## Minimum device support

- PC: Windows 10
- Mac: High Sierra
- Android: any device that supports Chrome 79.x
- iOS: Phone 6/7/8/8P/X and iPad

**[⬆ Back to top](#table-of-contents)**

# Testing

## Browser and device testing

### Chrome testing on Mac/iOS/Windows/Android

Chrome is free software available to download on the World Wide Web. Ensure the
version of Chrome meets the [Minimum browser support](#minimum-browser-support)
for Chrome.

**[Download Chrome](https://www.google.com/chrome/)**

### Edge testing on Mac/iOS/Windows/Android

Edge is free software available to download on the World Wide Web. Ensure the
version of Edge meets the [Minimum browser support](#minimum-browser-support)
for Edge.

**[Download Edge](https://www.microsoft.com/en-us/edge)**

### Firefox testing on Mac/iOS/Windows/Android

Firefox is free software available to download on the World Wide Web. Ensure the
version of Firefox meets the [Minimum browser support](#minimum-browser-support)
for Firefox.

**[Download Firefox](https://www.mozilla.org/en-US/firefox/)**

### iOS device testing on a Mac

The developer software called **Xcode** can be downloaded and installed for free
at:

**[https://apps.apple.com/ca/app/xcode/id497799835?mt=12](https://apps.apple.com/ca/app/xcode/id497799835?mt=12)**

Once installed, you can use the **Simulator** feature to test in all the latest
and greatest devices.

### Safari testing on a Mac/iOS

Safari comes pre-installed in Mac computers and iOS devices. Ensure the version
of Safari meets the [Minimum browser support](#minimum-browser-support) for
Safari.

**[⬆ Back to top](#table-of-contents)**

# Code quality

All of our projects that live in a production environment must be tested and
operate to a minimum QA level of _quality_.

**NOTE:** QA level may vary from project to project, be sure to check with the team or project leader before shipping anything to production:

A single web page's expectations of "quality":

- [ ] "Not Broken" - Page operates and serves its purpose (e.g. page gives a 200 response, links to scripts and CSS are also 200)
- [ ] "Clean UI" - Page does not look broken or contain framework/server-side error messages
- [ ] "No Console Errors" - Page contains no errors in Console (warnings are permitted)
- [ ] "W3C Valid" - Page source is tested with the W3C Markup Validation Service (https://validator.w3.org/) and passes with minimal warnings (best judgement) and 0 errors
- [ ] "Lighthouse" - Page is tested with Lighthouse (https://web.dev/measure) (web app or browser extension) and passes a minimum score of 70 for Performance, Accessibility, Best Practices, and SEO
- [ ] "Accessibility" - Page can be navigated by using a keyboard and all interactive elements are accessible by using the spacebar and/or Enter/Return buttons.

3rd party libraries that impact production performance must be taken into consideration but are not counted towards this minimum score of 70.

## General Principals

- Don't rely on `:hover`, or mouseover events to get to content

## General Methodologies

- Prettier file (link to `.prettierrc`)

### "Mobile-first" development

Try the best practice of developing web pages "mobile-first" by testing 
synchronously in a browser or emulator that is set to a minimum screen width of 
**375px**.

> "Writing front-end code without considering mobile doesn't cut the mustard, it
> cuts the cheese."
>
> _[yellowshoe.com.au/standards/](https://yellowshoe.com.au/standards/)_

#### Hierarchy of audience

  1. Mobile (no breakpoint)
  2. Tablet (768px breakpoint)
  3. Desktop (1024px breakpoint)

#### Gesture-first mind-set

There is no "click", "hover", "on mouseover", "mouseout", "mouse 
x/y coordinate", "scrollbar", and no "scroll" events; tailor your code towards this experience 
first before worrying about pointer/mouse events. 

**For example:** if you need to develop an interactive experience where 
information or content is "gated" (visibly hidden or not available to the DOM) 
by requiring the user to first **_mouse over_** an element, a user without a 
mouse will never be able to access this gated content. Instead, allow the gated
content to be activated by click or selection.

**[⬆ Back to top](#table-of-contents)**

# HTML

## HTML principles

- If it's a heading use a heading `<h1>`, `<h2>`, `<h3>`, `<h4>`
- If it's tabular data use a `<table>`
- If it's a list then use `<ul>` or `<ol>`
  - `<ul>` lists should contain items where it doesn't matter which order they 
  are in
  - `<ol>` lists should contain items where the order they appear in 
  **absolutely matters**
- HTML should work without the presence of CSS or Javascript (content should be
  accessible, form submissions should work, the HTML on it's own should have
  value)
- Never choose a heading level based on styling; if a heading doesn't look
  correct to design specs, raise the issue with your team

## HTML tools

- Use our team's [ESLint file](eslint/test-files/.eslintrc.js) (includes Prettier rules) in 
  projects to automatically format your HTML to our guide's standards.
  [Read more about Prettier](https://prettier.io/docs/en/index.html).
- [HTML 5 Outliner](https://gsnedders.html5.org/outliner/) can be utilized to 
  understand how readable and accessible your site's content is when boiled down
  to it's core without markup, style, and functionality
- [W3C Markup Validation Service](https://validator.w3.org/) can be utilized to 
  gauge how valid the markup you're publishing is

## HTML syntax

- Limit HTML files width to 80 characters
- Use lower case tags with double quote attributes
  
  ```html
  <!-- Avoid -->
  <a href='https://domain.com/'>Visit our site</a>
  <a href=https://domain.com/>Visit our site</a>
  <A HREF="https://domain.com/">Visit our site</A>

  <!-- Good example -->
  <a href="https://domain.com/">Visit our site</a>
  ```

- Use soft indents of two spaces
- HTML5 `<!doctype html>`
- The `lang` property of `<html>` should be correct to the
  [localization](#Localization) of the page content
- Do not use the `class` property in the `<html>` tag e.g.
  `<html class="no-js lt-ie9">`
- Do not use IE's non-standard
  [conditional comments](<https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/compatibility/ms537512(v=vs.85)?redirectedfrom=MSDN>)
  e.g. `<!--[if IE 8]> <html class="no-js lt-ie9"> <![endif]-->`
- Use `utf-8` character encoding `<meta charset="utf-8">`
- Do not use `<meta http-equiv="X-UA-Compatible" content="IE=edge">`
  ([Minimum browser support](#minimum-browser-support))
- Use `<em>` and `<strong>`; do not use `<i>` or `<b>`
- Use as few `<span>` and `<div>` elements as possible (the leaner the HTML is,
  the easier it is to work with)
- Avoid leaving a trailing slash on void/empty HTML elements (no longer
  necessary):

  ```html
  <!-- Avoid -->
  <br />
  <hr />
  <img />
  <input />
  <link />
  <meta />

  <!-- Good -->
  <br>
  <hr>
  <img>
  <input>
  <link>
  <meta>
  ```

- Nesting rules:

  - Write elements without attributes on one line:

  ```html
  <p>The quick brown fox jumps.</p>
  ```

  - Write elements with attributes nested:

  ```html
  <p class="lead">
    The quick brown fox jumps.
  </p>
  ```

  - Write elements with multi-line content nested:

  ```html
  <p>
    The quick brown fox jumps. Do or do not — there is no try.
  </p>
  ```

- Use a single blank line to break up complex hierarchies. Separate child
  elements with a single blank line.

  ```html
  <ul>
    <li>
      <h2>Title</h2>
      <p>Lorem ipsum dolor.</p>
    </li>

    <li>
      <h2>Title</h2>
      <p>Lorem ipsum dolor.</p>
    </li>

    <li>
      <h2>Title</h2>
      <p>Lorem ipsum dolor.</p>
    </li>
  </ul>
  ```

- Keep `<script>` files one line above `</body>`

  ```html
  <!-- Avoid #1 -->
  <body>
    ...
    <h1>Welcome to the site</h1>
    ...
    <script src="js/main.js"></script>
    <footer>
    ...
    </footer>
  </body>
  </html>


  <!-- Avoid #2 -->
  <body>
    ...
    <h1>Welcome to the site</h1>
    ...
    <script src="js/main.js"></script>
    <footer>
    ...
    </footer>
  </body>
  </html>

  <!-- Avoid #3 -->
    ...
    <script src="js/main.js"></script>
  </head>
  <body>
    ...
    <h1>Welcome to the site</h1>
    ...
    <footer>
    ...
    </footer>
  </body>
  </html>

  <!-- Good example -->
  <body>
    ...
    <h1>Welcome to the site</h1>
    ...
    <footer>
    ...
    </footer>
    <script src="js/main.js"></script>
  </body>
  </html>
  ```

- Do not specify a type when including CSS and JavaScript files e.g. `text/css`
  and `text/javascript`
- Do not use the `style` property on tags with the exception of
  `style="display:none;"` when necessary for functional cases e.g. modals,
  alerts, gated content
- Attributes in HTML start tags must be separated from each other by one space

  ```html
  <!-- Avoid -->
  <input  type="checkbox" value="1" checked>

  <!-- Good example -->
  <input type="checkbox" value="1" checked>
  ```

- HTML end tags must contain no spaces

  ```html
  <!-- Avoid -->
  <p>
    The quick brown fox jumps.
  </p >

  <!-- Good example -->
  <p>
    The quick brown fox jumps.
  </p>
  ```

- The order of attributes in a tag:

  - Critical attributes first e.g. `src`, `href`, `type`
  - `class` should always be last, except for images: `alt` should be last in
    order for images
  - `data-*` attributes should be placed before `class` and after critical
    attributes
  - everything else should be alphabetized between critical attributes and
    `data-*`

  ```html
  <!-- Avoid -->
  <input
    class=""
    type="text"
    id=""
    name=""
    value=""
    placeholder=""
    readonly
    disabled
  />

  <!-- Good example -->
  <input
    type="text"
    disabled
    id=""
    name=""
    placeholder=""
    readonly
    value=""
    class=""
  />
  ```

- When an element has too many attributes it’s hard to read; put attributes on
  separate lines with a 2 space indent on the attributes:

  ```html
  <button
    type="button"
    class="button"
    id="coordinates-button"
    data-loading="Loading..."
    data-x="123"
    data-y="789"
  >
    Send Coordinates
  </button>
  ```

- Boolean attributes must contain no value:

  ```html
  <!-- Avoid -->
  <input type="checkbox" value="1" checked="checked" />

  <input type="text" disabled="disabled" />

  <select>
    <option value="1" selected="selected">1</option>
  </select>

  <!-- Good example -->
  <input type="checkbox" value="1" checked>

  <input type="text" disabled>

  <select>
    <option value="1" selected>1</option>
  </select>
  ```

- JavaScript generated markup must adhere to the same HTML syntax rules

**[⬆ Back to top](#table-of-contents)**

# CSS

## CSS methodology

- Do not use `!important`
  - Exceptions: when there is a 3rd party stylesheet that contains a very 
  specific selector or uses `!important` and you need to override, please flag 
  this with your team or in your code review and add `!important` as needed.
- Do not create specific/nested selectors (this can easily lead to UI regression
  issues); instead make reuseable styles that fulfill a design pattern

  ```css
  /* Avoid */
  .list__articles li a {
    text-decoration: none;
  }

  /* Good example */
  /* Use a utility class that lives in a utility specific CSS file/framework */
  .text-decoration--none {
    text-decoration: none;
  }

  /*
  * Example HTML with class applied
  
  <ul class="list__articles">
    <li>
      <a href="#" class="text-decoration--none">Article Title</a>
    </li>
  </ul>
  */
  ```

- Declaration order: related property declarations should be grouped together
  following the order:

  1. Positioning
  1. Box model
  1. Typographic
  1. Visual
  1. Misc

  Positioning comes first because it can remove an element from the normal flow
  of the document and override box model related styles. The box model comes
  next as it dictates a component's dimensions and placement.

  Everything else takes place inside the component or without impacting the
  previous two sections, and thus they come last.

  ```css
  .declaration-order {
    /* Positioning */
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    z-index: 100;

    /* Box-model */
    display: block;
    float: right;
    width: 100px;
    height: 100px;

    /* Typography */
    font: 400 16px Helvetica, Arial, sans-serif;
    line-height: 1.5;
    color: #393a3d;
    text-align: center;

    /* Visual */
    background-color: #fff;
    border: 1px solid #393a3d;
    border-radius: 3px;

    /* Misc */
    opacity: 1;
  }
  ```

- Use SASS for compiling production CSS whenever possible to avoid use of
  `@import` and multiple `<link>` elements
- Media queries we support are `368px` ("Small" or "Mobile"), `768px` ("Large"
  or "Tablet"), and `1024px` ("Large" or "Desktop")
- Keep CSS completely separate from HTML
- Create re-useable classes and avoid unique classes that do the same thing
- Long-hand syntax is totally fine; readable code is better code
- Use lower-case
  [Two Dashes style BEM naming convention](https://en.bem.info/methodology/naming-convention/#two-dashes-style):

  - Names are written in lowercase Latin letters.
  - Words within the names of BEM entities are separated by a hyphen `-`.
  - The element name is separated from the block name by a double underscore
    `__`.
  - Boolean modifiers are separated from the name of the block or element by a
    double hyphen `--`.
  - The value of a modifier is separated from its name by a double hyphen `--`.

  ```css
  /* Avoid */
  .CTA_green {
    ...;
  }

  .disabled-submit {
    ...;
  }

  /* BEM naming convention */
  .block-name__elem-name--mod-name--mod-val {
    ...;
  }

  /* Good examples */
  .button--brand {
    ...;
  }

  .form__submit--disabled {
    ...;
  }
  ```

  **EXCEPTION CASE:** Design systems or component libraries will have their own
  naming conventions that can override this rule.

- Never use IDs for styling because IDs must be unique per document and are a
  shared concern with hyperlinks and JavaScript

  ```css
  /* Avoid */
  #form .input__name {
    ...;
  }

  /* Good example */
  /* Be very specific if you need to isolate a section of styling */
  .contact-form-en-ca .input__name {
    ...;
  }
  ```

- Don’t use element qualification e.g.

  ```css
  /* Avoid */
  ol.breadcrumbs {
    ...;
  }

  /* Good example */
  .breadcrumbs__list {
    ...;
  }
  ```

  - **Animations**: When it comes to making decisions on animation, please keep 
  the following in mind:

  > Animating well is core to a great web experience. You should always look to 
  avoid animating properties that will trigger layout or paints, both of which 
  are expensive and may lead to skipped frames. Declarative animations are 
  preferable to imperative since the browser has the opportunity to optimize 
  ahead of time.
  >
  > Today transforms are the best properties to animate because the GPU can 
  assist with the heavy lifting, so where you can limit your animations to 
  these, do so.
  >   - opacity
  >   - translate
  >   - rotate
  >   - scale
  >
  > _[High Performance Animations](https://www.html5rocks.com/en/tutorials/speed/high-performance-animations/)_

**[⬆ Back to top](#table-of-contents)**

## CSS syntax

- Limit CSS files width to 80 characters
- Use soft indents of two spaces
- Opening curly-brace on the same line as the selector, one space after
  selector, closing curly-brace on new line, and one blank line after closing
  curly-brace

  ```css
  button {
    ...;
  }

  img {
    ...;
  }
  ```

- Include one space after `:` for each declaration.
- When grouping selectors, keep individual selectors to a single line (more
  accurate error reporting) and double quotes on attributes

  ```css
  /* Avoid  */
  .selector, .selector-secondary, .selector[type='text'] {
    ...;
  }

  /* Good example */
  .selector,
  .selector-secondary,
  .selector[type="text"] {
    ...;
  }
  ```

- End all declarations with a semi-colon
- Avoid including spaces after commas within `rgb()`, `rgba()`, `hsl()`,
  `hsla()`, or `rect()` values
- Prefix property values with a leading zero e.g. 
  
  ```css
  /* Avoid */
  .selector {
    opacity: .5;
  }

  /* Good example */
  .selector {
    opacity: 0.5;
  }
  ```

- Lowercase all hex values e.g. `#fff`
- Use shorthand hex values where possible e.g. `#fff` instead of `#ffffff`
- Quote attribute values in selectors e.g. `input[type="text"]`
- Avoid specifying units for zero values e.g. `margin: 0;` instead of
  `margin: 0px;` (for zero lengths the unit identifier is optional)
- Place media queries as close to their relevant rule sets whenever possible
  (don't bundle them all in a separate stylesheet or at the end of the document)

  ```css
  .element {
    ...;
  }
  .element-avatar {
    ...;
  }
  .element-selected {
    ...;
  }

  @media (min-width: 768px) {
    .element {
      ...;
    }
    .element-avatar {
      ...;
    }
    .element-selected {
      ...;
    }
  }
  ```

- Do not one-line single declarations e.g.

  ```css
  /* Avoid */
  .element { margin-bottom: 20px; }

  /* Good example */
  .element {
    margin-bottom: 20px;
  }
  ```

- Limit shorthand declaration usage to instances where you must explicitly set
  all available values

  > Why? Shorthand is less readable (it requires additional 
  mental overhead), the sequence is easily done incorrectly, and it can override 
  other style rules lower in the cascade.

  ```css
  /* Bad example */
  .element {
    margin: 0 0 10px;
    background: red;
    background: url("image.jpg");
    border-radius: 3px 3px 0 0;
  }

  /* Good example */
  .element {
    margin-bottom: 10px;
    background-color: red;
    background-image: url("image.jpg");
    border-top-left-radius: 3px;
    border-top-right-radius: 3px;
  }
  ```

- There are only two approved media queries:

  ```css
  /* Tablet and up */
  @media (min-width: 768px) {
    ...;
  }
  /* Desktop and up */
  @media (min-width: 1024px) {
    ...;
  }
  ```

  Anything else should be flagged and raised as an issue with your team.

  > The first media query is no media query.
  >
  > _Ethan Marcotte_

- String literals should be single-quoted e.g.

  ```css
  /* Avoid */
  font-family: "Helvetica", "Arial", sans-serif;
  font-family: Helvetica, Arial, sans-serif;

  background-image: url("/images/eye-of-sauron.jpg");
  background-image: url(/images/eye-of-sauron.jpg);

  content: "Frodo";

  /* Good examples */
  font-family: 'Helvetica', 'Arial', sans-serif;

  background-image: url('/images/eye-of-sauron.jpg');

  content: 'Frodo';
  ```

## CSS tools

- Use [SASS](https://sass-lang.com/) for compiling production CSS whenever
  possible
- [CSS Stats](https://cssstats.com/): stats for your CSS!

## CSS frameworks

- We currently do not use or endorse any CSS frameworks

**[⬆ Back to top](#table-of-contents)**

# SASS

## SASS methodologies

- SASS files end with `.scss`
- You can say "SASS" or "S.C.S.S." - whatever tickles your fancy
- Limit SCSS files width to 80 characters
- SASS module files live with their corresponding `.js` that calls them e.g.

  ```bash
  /src
    /components
      /Button
        index.js
        index.module.scss
  ```

- Architecture of files and the order of importing them should follow this 
  pattern:

  ```bash
  sass/
  |
  |– abstracts/
  |   |– _variables.scss    # Sass Variables
  |   |– _functions.scss    # Sass Functions
  |   |– _mixins.scss       # Sass Mixins
  |
  |– base/
  |   |– _reset.scss        # Reset/normalize
  |   |– _typography.scss   # Typography rules
  |   …                     # Etc.
  |
  |– layout/
  |   |– _grid.scss         # Grid system
  |   |– _spacers_.scss     # Header
  |
  |– vendors/
  |   |– _bootstrap.scss    # Bootstrap
  |   |– _jquery-ui.scss    # jQuery UI
  |   …                     # Etc.
  |
  |– main.scss              # Main Sass file
  ```

  **Abstracts Folder**
  
  The `abstracts/` folder gathers all Sass tools and helpers used across the 
  project. Every global variable, function, mixin and placeholder should be put 
  in here.

  The rule of thumb for this folder is that it should not output a single line 
  of CSS when compiled on its own. These are nothing but Sass helpers.

  **Base Folder**

  The `base/` folder holds boilerplate code for the project. In there, you'll 
  find files like a reset file, typographic rules, and probably a stylesheet 
  defining some standard styles for commonly used HTML elements (_base.scss).

  **Layout Folder**

  The `layout/` folder contains everything that takes part in laying out the 
  site or application. This folder will have SASS files for spacers and grid.

  **Vendors Folder**

  The `vendors/` folder should contain all the SASS/CSS files from external 
  libraries and frameworks that your project uses.

  **Additional folders**

  Other folders that should be considered depending on project requirements 
  would be Components, Pages, and Themes.

  **Main.scss**

  This file should only contain comments and imports and follow these 
  guidelines:

  - one file per `@import`;
  - one `@import` per line;
  - no new line between two imports from the same folder;
  - a new line after the last import from a folder;
  - file extensions and leading underscores omitted.

  ```scss
  @import 'abstracts/variables';
  @import 'abstracts/functions';
  @import 'abstracts/mixins';

  @import 'base/reset';
  @import 'base/typography';

  @import 'layout/grid';
  @import 'layout/spacers';

  @import 'vendors/bootstrap';
  @import 'vendors/jquery-ui';
  ```

### File Naming

- An `.scss` file starting with an underscore `_` is a file that is imported. 
Files that do not start with an underscore should be files that are compiled 
as their own .css file. For example from the structure listed above, the final 
compiled output is a `main.css` file.
- All files should be lowercase and hyphenated.
- If a file contains multiple variations of a selector, make sure the file is 
named plurally e.g. `buttons.scss` and not `button.scss` since it is 
unlikely that you will only ever have one button style. Context is important
for readability and quick comprehension.

**[⬆ Back to top](#table-of-contents)**

## SASS syntax

- Remove empty brackets

  ```scss
  /* Avoid */
  @include body02();

  /* Good example */
  @include body02;
  ```

- Prefix property values with a leading zero
  
  ```scss
  /* Avoid */
  .selector {
    opacity: .5;
  }

  /* Good example */
  .selector {
    opacity: 0.5;
  }
  ```

- Avoid specifying units for zero values e.g. `margin: 0;` instead of
  `margin: 0px;`

  > Why? For zero lengths, the unit identifier is optional

- Calculations should always be wrapped in parentheses with a single space 
  between values

  > Why? Improves readability and also prevents some edge cases by forcing SASS 
  to evaluate the contents of the parentheses

  ```scss
  /* Avoid */
  .selector {
    width: 100%/3;
  }

  /* Good example */
  .selector {
    width: (100% / 3);
  }  
  ```
  
- Nest only pseudo-classes and pseudo-elements within the initial selector

  ```scss
  /* Avoid */
  .selector {
    &--active {
      /*
        poor readability and easily missed in refactor or debugging 
        e.g searching for 'selector--active' will return no results
      */
      color: #fff;
    }

    .disabled {
      /*
        .disabled or other modifiers are restricted space for utility classes
      */
    }

    &:hover {
      color: #fff;
    }

    &::before {
      content: 'pseudo-element'
    }
  }

  /* Good example */
  .selector {
    &:hover {
      color: #fff;
    }

    &::before {
      content: 'pseudo-element'
    }
  }

  .selector--active {
    color: #fff;
  }
  ```

- SASS variable, function, and mixin naming convention is camel case and make it
meaningful
  
  ```scss
  /* Avoid */
  $desk: 1024px;
  $font: "Helvetica", "Arial", sans-serif;

  @mixin bg-dark {
    background-color: $grey08;
  }

  /* Good example */
  $desktopBreakpoint: 1024px;
  $fontFamily: "Helvetica", "Arial", sans-serif;

  @mixin backgroundColorDark {
    background-color: $grey08;
  }
  ```

**[⬆ Back to top](#table-of-contents)**

# JavaScript

## JavaScript principals

- Our team follows functional programming practices

  > Functional programming is a programming paradigm — a style of building the
  > structure and elements of computer programs — that treats computation as the
  > evaluation of mathematical functions and avoids changing-state and mutable
  > data
  >
  > _Wikipedia_

- Our team's JavaScript functions follow the
  [Single Responsibility Principle](https://en.wikipedia.org/wiki/Single_responsibility_principle)

  > A class should have one, and only one, reason to change.
  >
  > _Robert C. Martin_

- Our JavaScript's global scope is clean and we put code into namespaces

## Types

- **Primitives**: When you access a primitive type you work directly on its value.

  - `string`
  - `number`
  - `boolean`
  - `null`
  - `undefined`
  - `symbol`

  ```javascript
  const foo = 1;
  let bar = foo;

  bar = 9;

  console.log(foo, bar); // => 1, 9
  ```

  > Why? Symbols cannot be faithfully polyfilled, so they should not be used
  > when targeting browsers/environments that don’t support them natively.

- **Complex**: When you access a complex type you work on a reference to its value.

  - `object`
  - `array`
  - `function`

  ```javascript
  const foo = [1, 2];
  const bar = foo;

  bar[0] = 9;

  console.log(foo[0], bar[0]); // => 9, 9
  ```

**[⬆ Back to top](#table-of-contents)**

## References

- Use `const` for all of your references; avoid using `var`. eslint: [`prefer-const`](https://eslint.org/docs/rules/prefer-const.html), [`no-const-assign`](https://eslint.org/docs/rules/no-const-assign.html)

  > Why? This ensures that you can’t reassign your references, which can lead to
  > bugs and difficult to comprehend code.

  ```javascript
  // bad
  var a = 1;
  var b = 2;

  // good
  const a = 1;
  const b = 2;
  ```

- If you must reassign references, use `let` instead of `var`. eslint: [`no-var`](https://eslint.org/docs/rules/no-var.html)

  > Why? `let` is block-scoped rather than function-scoped like `var`.

  ```javascript
  // bad
  var count = 1;
  if (true) {
    count += 1;
  }

  // good, use the let.
  let count = 1;
  if (true) {
    count += 1;
  }
  ```

- Note that both `let` and `const` are block-scoped.

  ```javascript
  // const and let only exist in the blocks they are defined in.
  {
    let a = 1;
    const b = 1;
  }
  console.log(a); // ReferenceError
  console.log(b); // ReferenceError
  ```

**[⬆ Back to top](#table-of-contents)**

## Objects

- Use the literal syntax for object creation. eslint: [`no-new-object`](https://eslint.org/docs/rules/no-new-object.html)

  ```javascript
  // bad
  const item = new Object();

  // good
  const item = {};
  ```

- Use computed property names when creating objects with dynamic property names.

  > Why? They allow you to define all the properties of an object in one place.

  ```javascript

  function getKey(k) {
    return `a key named ${k}`;
  }

  // bad
  const obj = {
    id: 5,
    name: 'San Francisco',
  };
  obj[getKey('enabled')] = true;

  // good
  const obj = {
    id: 5,
    name: 'San Francisco',
    [getKey('enabled')]: true,
  };
  ```

- Use object method shorthand. eslint: [`object-shorthand`](https://eslint.org/docs/rules/object-shorthand.html)

  ```javascript
  // bad
  const atom = {
    value: 1,

    addValue: function (value) {
      return atom.value + value;
    },
  };

  // good
  const atom = {
    value: 1,

    addValue(value) {
      return atom.value + value;
    },
  };
  ```

- Use property value shorthand. eslint: [`object-shorthand`](https://eslint.org/docs/rules/object-shorthand.html)

  > Why? It is shorter and descriptive.

  ```javascript
  const lukeSkywalker = 'Luke Skywalker';

  // bad
  const obj = {
    lukeSkywalker: lukeSkywalker,
  };

  // good
  const obj = {
    lukeSkywalker,
  };
  ```

- Group your shorthand properties at the beginning of your object declaration.

  > Why? It’s easier to tell which properties are using the shorthand.

  ```javascript
  const anakinSkywalker = 'Anakin Skywalker';
  const lukeSkywalker = 'Luke Skywalker';

  // bad
  const obj = {
    episodeOne: 1,
    twoJediWalkIntoACantina: 2,
    lukeSkywalker,
    episodeThree: 3,
    mayTheFourth: 4,
    anakinSkywalker,
  };

  // good
  const obj = {
    lukeSkywalker,
    anakinSkywalker,
    episodeOne: 1,
    twoJediWalkIntoACantina: 2,
    episodeThree: 3,
    mayTheFourth: 4,
  };
  ```

- Only quote properties that are invalid identifiers. eslint: [`quote-props`](https://eslint.org/docs/rules/quote-props.html)

  > Why? In general we consider it subjectively easier to read. It improves
  > syntax highlighting, and is also more easily optimized by many JS engines.

  ```javascript
  // bad
  const bad = {
    'foo': 3,
    'bar': 4,
    'data-blah': 5,
  };

  // good
  const good = {
    foo: 3,
    bar: 4,
    'data-blah': 5,
  };
  ```

- Do not call `Object.prototype` methods directly, such as `hasOwnProperty`,
`propertyIsEnumerable`, and `isPrototypeOf`. eslint: [`no-prototype-builtins`](https://eslint.org/docs/rules/no-prototype-builtins)

  > Why? These methods may be shadowed by properties on the object in question -
  >consider `{ hasOwnProperty: false }` - or, the object may be a null object
  > (`Object.create(null)`).

  ```javascript
  // bad
  console.log(object.hasOwnProperty(key));

  // good
  console.log(Object.prototype.hasOwnProperty.call(object, key));

  // best
  const has = Object.prototype.hasOwnProperty; // cache the lookup once, in module scope.
  console.log(has.call(object, key));
  /* or */
  import has from 'has'; // https://www.npmjs.com/package/has
  console.log(has(object, key));
  ```

- Prefer the object spread operator over [`Object.assign`](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Object/assign)
to shallow-copy objects. Use the object rest operator to get a new object with
certain properties omitted.

  ```javascript
  // very bad
  const original = { a: 1, b: 2 };
  const copy = Object.assign(original, { c: 3 }); // this mutates `original` ಠ_ಠ
  delete copy.a; // so does this

  // bad
  const original = { a: 1, b: 2 };
  const copy = Object.assign({}, original, { c: 3 }); // copy => { a: 1, b: 2, c: 3 }

  // good
  const original = { a: 1, b: 2 };
  const copy = { ...original, c: 3 }; // copy => { a: 1, b: 2, c: 3 }

  const { a, ...noA } = copy; // noA => { b: 2, c: 3 }
  ```

**[⬆ Back to top](#table-of-contents)**

## Arrays

- Use the literal syntax for array creation. eslint: [`no-array-constructor`](https://eslint.org/docs/rules/no-array-constructor.html)

  ```javascript
  // bad
  const items = new Array();

  // good
  const items = [];
  ```

- Use [Array#push](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Array/push)
instead of direct assignment to add items to an array.

  ```javascript
  const someStack = [];

  // bad
  someStack[someStack.length] = 'abracadabra';

  // good
  someStack.push('abracadabra');
  ```

- Use array spreads `...` to copy arrays.

  ```javascript
  // bad
  const len = items.length;
  const itemsCopy = [];
  let i;

  for (i = 0; i < len; i += 1) {
    itemsCopy[i] = items[i];
  }

  // good
  const itemsCopy = [...items];
  ```

- To convert an iterable object to an array, use spreads `...` instead of [`Array.from`](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Array/from).

  ```javascript
  const foo = document.querySelectorAll('.foo');

  // good
  const nodes = Array.from(foo);

  // best
  const nodes = [...foo];
  ```

- Use [`Array.from`](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Array/from) for converting an array-like object to an array.

  ```javascript
  const arrLike = { 0: 'foo', 1: 'bar', 2: 'baz', length: 3 };

  // bad
  const arr = Array.prototype.slice.call(arrLike);

  // good
  const arr = Array.from(arrLike);
  ```

- Use [`Array.from`](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Array/from) instead of spread `...` for mapping over iterables, because it avoids creating an intermediate array.

  ```javascript
  // bad
  const baz = [...foo].map(bar);

  // good
  const baz = Array.from(foo, bar);
  ```

- Use return statements in array method callbacks. It’s ok to omit the return if the function body consists of a single statement returning an expression without side effects, following [8.2](#arrows--implicit-return). eslint: [`array-callback-return`](https://eslint.org/docs/rules/array-callback-return)

  ```javascript
  // good
  [1, 2, 3].map((x) => {
    const y = x + 1;
    return x * y;
  });

  // good
  [1, 2, 3].map((x) => x + 1);

  // bad - no returned value means `acc` becomes undefined after the first iteration
  [[0, 1], [2, 3], [4, 5]].reduce((acc, item, index) => {
    const flatten = acc.concat(item);
  });

  // good
  [[0, 1], [2, 3], [4, 5]].reduce((acc, item, index) => {
    const flatten = acc.concat(item);
    return flatten;
  });

  // bad
  inbox.filter((msg) => {
    const { subject, author } = msg;
    if (subject === 'Mockingbird') {
      return author === 'Harper Lee';
    } else {
      return false;
    }
  });

  // good
  inbox.filter((msg) => {
    const { subject, author } = msg;
    if (subject === 'Mockingbird') {
      return author === 'Harper Lee';
    }

    return false;
  });
  ```

- Use line breaks after open and before close array brackets if an array has multiple lines

  ```javascript
  // bad
  const arr = [
    [0, 1], [2, 3], [4, 5],
  ];

  const objectInArray = [{
    id: 1,
  }, {
    id: 2,
  }];

  const numberInArray = [
    1, 2,
  ];

  // good
  const arr = [[0, 1], [2, 3], [4, 5]];

  const objectInArray = [
    {
      id: 1,
    },
    {
      id: 2,
    },
  ];

  const numberInArray = [
    1,
    2,
  ];
  ```

**[⬆ Back to top](#table-of-contents)**

## Destructuring

- Use object destructuring when accessing and using multiple properties of an object. eslint: [`prefer-destructuring`](https://eslint.org/docs/rules/prefer-destructuring)

  > Why? Destructuring saves you from creating temporary references for those properties.

  ```javascript
  // bad
  function getFullName(user) {
    const firstName = user.firstName;
    const lastName = user.lastName;

    return `${firstName} ${lastName}`;
  }

  // good
  function getFullName(user) {
    const { firstName, lastName } = user;
    return `${firstName} ${lastName}`;
  }

  // best
  function getFullName({ firstName, lastName }) {
    return `${firstName} ${lastName}`;
  }
  ```

- Use array destructuring. eslint: [`prefer-destructuring`](https://eslint.org/docs/rules/prefer-destructuring)

  ```javascript
  const arr = [1, 2, 3, 4];

  // bad
  const first = arr[0];
  const second = arr[1];

  // good
  const [first, second] = arr;
  ```

- Use object destructuring for multiple return values, not array destructuring.

  > Why? You can add new properties over time or change the order of things without breaking call sites.

  ```javascript
  // bad
  function processInput(input) {
    // then a miracle occurs
    return [left, right, top, bottom];
  }

  // the caller needs to think about the order of return data
  const [left, __, top] = processInput(input);

  // good
  function processInput(input) {
    // then a miracle occurs
    return { left, right, top, bottom };
  }

  // the caller selects only the data they need
  const { left, top } = processInput(input);
  ```

**[⬆ Back to top](#table-of-contents)**

## Strings

- Use single quotes `''` for strings. eslint: [`quotes`](https://eslint.org/docs/rules/quotes.html)

  ```javascript
  // bad
  const name = "Capt. Janeway";

  // bad - template literals should contain interpolation or newlines
  const name = `Capt. Janeway`;

  // good
  const name = 'Capt. Janeway';
  ```

- Strings that cause the line to go over 100 characters should not be written across multiple lines using string concatenation.

  > Why? Broken strings are painful to work with and make code less searchable.

  ```javascript
  // bad
  const errorMessage = 'This is a super long error that was thrown because \
  of Batman. When you stop to think about how Batman had anything to do \
  with this, you would get nowhere \
  fast.';

  // bad
  const errorMessage = 'This is a super long error that was thrown because ' +
    'of Batman. When you stop to think about how Batman had anything to do ' +
    'with this, you would get nowhere fast.';

  // good
  const errorMessage = 'This is a super long error that was thrown because of Batman. When you stop to think about how Batman had anything to do with this, you would get nowhere fast.';
  ```

- When programmatically building up strings, use template strings instead of concatenation. eslint: [`prefer-template`](https://eslint.org/docs/rules/prefer-template.html) [`template-curly-spacing`](https://eslint.org/docs/rules/template-curly-spacing)

  > Why? Template strings give you a readable, concise syntax with proper newlines and string interpolation features.

  ```javascript
  // bad
  function sayHi(name) {
    return 'How are you, ' + name + '?';
  }

  // bad
  function sayHi(name) {
    return ['How are you, ', name, '?'].join();
  }

  // bad
  function sayHi(name) {
    return `How are you, ${ name }?`;
  }

  // good
  function sayHi(name) {
    return `How are you, ${name}?`;
  }
  ```

- Never use `eval()` on a string, it opens too many vulnerabilities. eslint: [`no-eval`](https://eslint.org/docs/rules/no-eval)

- Do not unnecessarily escape characters in strings. eslint: [`no-useless-escape`](https://eslint.org/docs/rules/no-useless-escape)

  > Why? Backslashes harm readability, thus they should only be present when necessary.

  ```javascript
  // bad
  const foo = '\'this\' \i\s \"quoted\"';

  // good
  const foo = '\'this\' is "quoted"';
  const foo = `my name is '${name}'`;
  ```

**[⬆ Back to top](#table-of-contents)**

## Functions

- Use named function expressions instead of function declarations. eslint: [`func-style`](https://eslint.org/docs/rules/func-style)

  > Why? Function declarations are hoisted, which means that it’s easy - too easy - to reference the function before it is defined in the file. This harms readability and maintainability. If you find that a function’s definition is large or complex enough that it is interfering with understanding the rest of the file, then perhaps it’s time to extract it to its own module! Don’t forget to explicitly name the expression, regardless of whether or not the name is inferred from the containing variable (which is often the case in modern browsers or when using compilers such as Babel). This eliminates any assumptions made about the Error’s call stack. ([Discussion](https://github.com/airbnb/javascript/issues/794))

  ```javascript
  // bad
  function foo() {
    // ...
  }

  // bad
  const foo = function () {
    // ...
  };

  // good
  // lexical name distinguished from the variable-referenced invocation(s)
  const short = function longUniqueMoreDescriptiveLexicalFoo() {
    // ...
  };
  ```

- Wrap immediately invoked function expressions in parentheses. eslint: [`wrap-iife`](https://eslint.org/docs/rules/wrap-iife.html)

  > Why? An immediately invoked function expression is a single unit - wrapping both it, and its invocation parens, in parens, cleanly expresses this. Note that in a world with modules everywhere, you almost never need an IIFE.

  ```javascript
  // immediately-invoked function expression (IIFE)
  (function () {
    console.log('Welcome to the Internet. Please follow me.');
  }());
  ```

- Never declare a function in a non-function block (`if`, `while`, etc). Assign the function to a variable instead. Browsers will allow you to do it, but they all interpret it differently, which is bad news bears. eslint: [`no-loop-func`](https://eslint.org/docs/rules/no-loop-func.html)

- **Note:** ECMA-262 defines a `block` as a list of statements. A function declaration is not a statement.

  ```javascript
  // bad
  if (currentUser) {
    function test() {
      console.log('Nope.');
    }
  }

  // good
  let test;
  if (currentUser) {
    test = () => {
      console.log('Yup.');
    };
  }
  ```

- Never name a parameter `arguments`. This will take precedence over the `arguments` object that is given to every function scope.

  ```javascript
  // bad
  function foo(name, options, arguments) {
    // ...
  }

  // good
  function foo(name, options, args) {
    // ...
  }
  ```

- Never use `arguments`, opt to use rest syntax `...` instead. eslint: [`prefer-rest-params`](https://eslint.org/docs/rules/prefer-rest-params)

  > Why? `...` is explicit about which arguments you want pulled. Plus, rest arguments are a real Array, and not merely Array-like like `arguments`.

  ```javascript
  // bad
  function concatenateAll() {
    const args = Array.prototype.slice.call(arguments);
    return args.join('');
  }

  // good
  function concatenateAll(...args) {
    return args.join('');
  }
  ```

- Use default parameter syntax rather than mutating function arguments.

  ```javascript
  // really bad
  function handleThings(opts) {
    // No! We shouldn’t mutate function arguments.
    // Double bad: if opts is falsy it'll be set to an object which may
    // be what you want but it can introduce subtle bugs.
    opts = opts || {};
    // ...
  }

  // still bad
  function handleThings(opts) {
    if (opts === void 0) {
      opts = {};
    }
    // ...
  }

  // good
  function handleThings(opts = {}) {
    // ...
  }
  ```

- Avoid side effects with default parameters.

  > Why? They are confusing to reason about.

  ```javascript
  var b = 1;
  // bad
  function count(a = b++) {
    console.log(a);
  }
  count();  // 1
  count();  // 2
  count(3); // 3
  count();  // 3
  ```

- Always put default parameters last.

  ```javascript
  // bad
  function handleThings(opts = {}, name) {
    // ...
  }

  // good
  function handleThings(name, opts = {}) {
    // ...
  }
  ```

- Never use the Function constructor to create a new function. eslint: [`no-new-func`](https://eslint.org/docs/rules/no-new-func)

  > Why? Creating a function in this way evaluates a string similarly to `eval()`, which opens vulnerabilities.

  ```javascript
  // bad
  var add = new Function('a', 'b', 'return a + b');

  // still bad
  var subtract = Function('a', 'b', 'return a - b');
  ```

- Spacing in a function signature. eslint: [`space-before-function-paren`](https://eslint.org/docs/rules/space-before-function-paren) [`space-before-blocks`](https://eslint.org/docs/rules/space-before-blocks)

  > Why? Consistency is good, and you shouldn’t have to add or remove a space when adding or removing a name.

  ```javascript
  // bad
  const f = function(){};
  const g = function (){};
  const h = function() {};

  // good
  const x = function () {};
  const y = function a() {};
  ```

- Never mutate parameters. eslint: [`no-param-reassign`](https://eslint.org/docs/rules/no-param-reassign.html)

  > Why? Manipulating objects passed in as parameters can cause unwanted variable side effects in the original caller.

  ```javascript
  // bad
  function f1(obj) {
    obj.key = 1;
  }

  // good
  function f2(obj) {
    const key = Object.prototype.hasOwnProperty.call(obj, 'key') ? obj.key : 1;
  }
  ```

- Never reassign parameters. eslint: [`no-param-reassign`](https://eslint.org/docs/rules/no-param-reassign.html)

  > Why? Reassigning parameters can lead to unexpected behavior, especially when accessing the `arguments` object. It can also cause optimization issues, especially in V8.

  ```javascript
  // bad
  function f1(a) {
    a = 1;
    // ...
  }

  function f2(a) {
    if (!a) { a = 1; }
    // ...
  }

  // good
  function f3(a) {
    const b = a || 1;
    // ...
  }

  function f4(a = 1) {
    // ...
  }
  ```

- Prefer the use of the spread operator `...` to call variadic functions. eslint: [`prefer-spread`](https://eslint.org/docs/rules/prefer-spread)

  > Why? It’s cleaner, you don’t need to supply a context, and you can not easily compose `new` with `apply`.

  ```javascript
  // bad
  const x = [1, 2, 3, 4, 5];
  console.log.apply(console, x);

  // good
  const x = [1, 2, 3, 4, 5];
  console.log(...x);

  // bad
  new (Function.prototype.bind.apply(Date, [null, 2016, 8, 5]));

  // good
  new Date(...[2016, 8, 5]);
  ```

- Functions with multiline signatures, or invocations, should be indented just like every other multiline list in this guide: with each item on a line by itself, with a trailing comma on the last item. eslint: [`function-paren-newline`](https://eslint.org/docs/rules/function-paren-newline)

  ```javascript
  // bad
  function foo(bar,
                baz,
                quux) {
    // ...
  }

  // good
  function foo(
    bar,
    baz,
    quux,
  ) {
    // ...
  }

  // bad
  console.log(foo,
    bar,
    baz);

  // good
  console.log(
    foo,
    bar,
    baz,
  );
  ```

**[⬆ Back to top](#table-of-contents)**

## Arrow Functions

- When you must use an anonymous function (as when passing an inline callback), use arrow function notation. eslint: [`prefer-arrow-callback`](https://eslint.org/docs/rules/prefer-arrow-callback.html), [`arrow-spacing`](https://eslint.org/docs/rules/arrow-spacing.html)

  > Why? It creates a version of the function that executes in the context of `this`, which is usually what you want, and is a more concise syntax.

  > Why not? If you have a fairly complicated function, you might move that logic out into its own named function expression.

  ```javascript
  // bad
  [1, 2, 3].map(function (x) {
    const y = x + 1;
    return x * y;
  });

  // good
  [1, 2, 3].map((x) => {
    const y = x + 1;
    return x * y;
  });
  ```

- If the function body consists of a single statement returning an [expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#Expressions) without side effects, omit the braces and use the implicit return. Otherwise, keep the braces and use a `return` statement. eslint: [`arrow-parens`](https://eslint.org/docs/rules/arrow-parens.html), [`arrow-body-style`](https://eslint.org/docs/rules/arrow-body-style.html)

  > Why? Syntactic sugar. It reads well when multiple functions are chained together.

  ```javascript
  // bad
  [1, 2, 3].map((number) => {
    const nextNumber = number + 1;
    `A string containing the ${nextNumber}.`;
  });

  // good
  [1, 2, 3].map((number) => `A string containing the ${number + 1}.`);

  // good
  [1, 2, 3].map((number) => {
    const nextNumber = number + 1;
    return `A string containing the ${nextNumber}.`;
  });

  // good
  [1, 2, 3].map((number, index) => ({
    [index]: number,
  }));

  // No implicit return with side effects
  function foo(callback) {
    const val = callback();
    if (val === true) {
      // Do something if callback returns true
    }
  }

  let bool = false;

  // bad
  foo(() => bool = true);

  // good
  foo(() => {
    bool = true;
  });
  ```

- In case the expression spans over multiple lines, wrap it in parentheses for better readability.

  > Why? It shows clearly where the function starts and ends.

  ```javascript
  // bad
  ['get', 'post', 'put'].map((httpMethod) => Object.prototype.hasOwnProperty.call(
      httpMagicObjectWithAVeryLongName,
      httpMethod,
    )
  );

  // good
  ['get', 'post', 'put'].map((httpMethod) => (
    Object.prototype.hasOwnProperty.call(
      httpMagicObjectWithAVeryLongName,
      httpMethod,
    )
  ));
  ```

- Always include parentheses around arguments for clarity and consistency. eslint: [`arrow-parens`](https://eslint.org/docs/rules/arrow-parens.html)

  > Why? Minimizes diff churn when adding or removing arguments.

  ```javascript
  // bad
  [1, 2, 3].map(x => x * x);

  // good
  [1, 2, 3].map((x) => x * x);

  // bad
  [1, 2, 3].map(number => (
    `A long string with the ${number}. It’s so long that we don’t want it to take up space on the .map line!`
  ));

  // good
  [1, 2, 3].map((number) => (
    `A long string with the ${number}. It’s so long that we don’t want it to take up space on the .map line!`
  ));

  // bad
  [1, 2, 3].map(x => {
    const y = x + 1;
    return x * y;
  });

  // good
  [1, 2, 3].map((x) => {
    const y = x + 1;
    return x * y;
  });
  ```

- Avoid confusing arrow function syntax (`=>`) with comparison operators (`<=`, `>=`). eslint: [`no-confusing-arrow`](https://eslint.org/docs/rules/no-confusing-arrow)

  ```javascript
  // bad
  const itemHeight = (item) => item.height <= 256 ? item.largeSize : item.smallSize;

  // bad
  const itemHeight = (item) => item.height >= 256 ? item.largeSize : item.smallSize;

  // good
  const itemHeight = (item) => (item.height <= 256 ? item.largeSize : item.smallSize);

  // good
  const itemHeight = (item) => {
    const { height, largeSize, smallSize } = item;
    return height <= 256 ? largeSize : smallSize;
  };
  ```

- Enforce the location of arrow function bodies with implicit returns. eslint: [`implicit-arrow-linebreak`](https://eslint.org/docs/rules/implicit-arrow-linebreak)

  ```javascript
  // bad
  (foo) =>
    bar;

  (foo) =>
    (bar);

  // good
  (foo) => bar;
  (foo) => (bar);
  (foo) => (
      bar
  )
  ```

**[⬆ Back to top](#table-of-contents)**

## Classes & Constructors

- Always use `class`. Avoid manipulating `prototype` directly.

  > Why? `class` syntax is more concise and easier to reason about.

  ```javascript
  // bad
  function Queue(contents = []) {
    this.queue = [...contents];
  }
  Queue.prototype.pop = function () {
    const value = this.queue[0];
    this.queue.splice(0, 1);
    return value;
  };

  // good
  class Queue {
    constructor(contents = []) {
      this.queue = [...contents];
    }
    pop() {
      const value = this.queue[0];
      this.queue.splice(0, 1);
      return value;
    }
  }
  ```

- Use `extends` for inheritance.

  > Why? It is a built-in way to inherit prototype functionality without breaking `instanceof`.

  ```javascript
  // bad
  const inherits = require('inherits');
  function PeekableQueue(contents) {
    Queue.apply(this, contents);
  }
  inherits(PeekableQueue, Queue);
  PeekableQueue.prototype.peek = function () {
    return this.queue[0];
  };

  // good
  class PeekableQueue extends Queue {
    peek() {
      return this.queue[0];
    }
  }
  ```

- Methods can return `this` to help with method chaining.

  ```javascript
  // bad
  Jedi.prototype.jump = function () {
    this.jumping = true;
    return true;
  };

  Jedi.prototype.setHeight = function (height) {
    this.height = height;
  };

  const luke = new Jedi();
  luke.jump(); // => true
  luke.setHeight(20); // => undefined

  // good
  class Jedi {
    jump() {
      this.jumping = true;
      return this;
    }

    setHeight(height) {
      this.height = height;
      return this;
    }
  }

  const luke = new Jedi();

  luke.jump()
    .setHeight(20);
  ```

- It’s okay to write a custom `toString()` method, just make sure it works successfully and causes no side effects.

  ```javascript
  class Jedi {
    constructor(options = {}) {
      this.name = options.name || 'no name';
    }

    getName() {
      return this.name;
    }

    toString() {
      return `Jedi - ${this.getName()}`;
    }
  }
  ```

- Classes have a default constructor if one is not specified. An empty constructor function or one that just delegates to a parent class is unnecessary. eslint: [`no-useless-constructor`](https://eslint.org/docs/rules/no-useless-constructor)

  ```javascript
  // bad
  class Jedi {
    constructor() {}

    getName() {
      return this.name;
    }
  }

  // bad
  class Rey extends Jedi {
    constructor(...args) {
      super(...args);
    }
  }

  // good
  class Rey extends Jedi {
    constructor(...args) {
      super(...args);
      this.name = 'Rey';
    }
  }
  ```

- Avoid duplicate class members. eslint: [`no-dupe-class-members`](https://eslint.org/docs/rules/no-dupe-class-members)

  > Why? Duplicate class member declarations will silently prefer the last one - having duplicates is almost certainly a bug.

  ```javascript
  // bad
  class Foo {
    bar() { return 1; }
    bar() { return 2; }
  }

  // good
  class Foo {
    bar() { return 1; }
  }

  // good
  class Foo {
    bar() { return 2; }
  }
  ```

- Class methods should use `this` or be made into a static method unless an external library or framework requires to use specific non-static methods. Being an instance method should indicate that it behaves differently based on properties of the receiver. eslint: [`class-methods-use-this`](https://eslint.org/docs/rules/class-methods-use-this)

  ```javascript
  // bad
  class Foo {
    bar() {
      console.log('bar');
    }
  }

  // good - this is used
  class Foo {
    bar() {
      console.log(this.bar);
    }
  }

  // good - constructor is exempt
  class Foo {
    constructor() {
      // ...
    }
  }

  // good - static methods aren't expected to use this
  class Foo {
    static bar() {
      console.log('bar');
    }
  }
  ```

**[⬆ Back to top](#table-of-contents)**

## Modules

- Always use modules (`import`/`export`) over a non-standard module system. You can always transpile to your preferred module system.

  > Why? Modules are the future, let’s start using the future now.

  ```javascript
  // bad
  const AirbnbStyleGuide = require('./AirbnbStyleGuide');
  module.exports = AirbnbStyleGuide.es6;

  // ok
  import AirbnbStyleGuide from './AirbnbStyleGuide';
  export default AirbnbStyleGuide.es6;

  // best
  import { es6 } from './AirbnbStyleGuide';
  export default es6;
  ```

- Do not use wildcard imports.

  > Why? This makes sure you have a single default export.

  ```javascript
  // bad
  import * as AirbnbStyleGuide from './AirbnbStyleGuide';

  // good
  import AirbnbStyleGuide from './AirbnbStyleGuide';
  ```

- And do not export directly from an import.

  > Why? Although the one-liner is concise, having one clear way to import and one clear way to export makes things consistent.

  ```javascript
  // bad
  // filename es6.js
  export { es6 as default } from './AirbnbStyleGuide';

  // good
  // filename es6.js
  import { es6 } from './AirbnbStyleGuide';
  export default es6;
  ```

- Only import from a path in one place.
eslint: [`no-duplicate-imports`](https://eslint.org/docs/rules/no-duplicate-imports)
  > Why? Having multiple lines that import from the same path can make code harder to maintain.

  ```javascript
  // bad
  import foo from 'foo';
  // … some other imports … //
  import { named1, named2 } from 'foo';

  // good
  import foo, { named1, named2 } from 'foo';

  // good
  import foo, {
    named1,
    named2,
  } from 'foo';
  ```

- Do not export mutable bindings.
eslint: [`import/no-mutable-exports`](https://github.com/benmosher/eslint-plugin-import/blob/master/docs/rules/no-mutable-exports.md)
  > Why? Mutation should be avoided in general, but in particular when exporting mutable bindings. While this technique may be needed for some special cases, in general, only constant references should be exported.

  ```javascript
  // bad
  let foo = 3;
  export { foo };

  // good
  const foo = 3;
  export { foo };
  ```

- In modules with a single export, prefer default export over named export.
eslint: [`import/prefer-default-export`](https://github.com/benmosher/eslint-plugin-import/blob/master/docs/rules/prefer-default-export.md)
  > Why? To encourage more files that only ever export one thing, which is better for readability and maintainability.

  ```javascript
  // bad
  export function foo() {}

  // good
  export default function foo() {}
  ```

- Put all `import`s above non-import statements.
eslint: [`import/first`](https://github.com/benmosher/eslint-plugin-import/blob/master/docs/rules/first.md)
  > Why? Since `import`s are hoisted, keeping them all at the top prevents surprising behavior.

  ```javascript
  // bad
  import foo from 'foo';
  foo.init();

  import bar from 'bar';

  // good
  import foo from 'foo';
  import bar from 'bar';

  foo.init();
  ```

- Multiline imports should be indented just like multiline array and object literals.

  > Why? The curly braces follow the same indentation rules as every other curly brace block in the style guide, as do the trailing commas.

  ```javascript
  // bad
  import {longNameA, longNameB, longNameC, longNameD, longNameE} from 'path';

  // good
  import {
    longNameA,
    longNameB,
    longNameC,
    longNameD,
    longNameE,
  } from 'path';
  ```

- Disallow Webpack loader syntax in module import statements.
eslint: [`import/no-webpack-loader-syntax`](https://github.com/benmosher/eslint-plugin-import/blob/master/docs/rules/no-webpack-loader-syntax.md)
  > Why? Since using Webpack syntax in the imports couples the code to a module bundler. Prefer using the loader syntax in `webpack.config.js`.

  ```javascript
  // bad
  import fooSass from 'css!sass!foo.scss';
  import barCss from 'style!css!bar.css';

  // good
  import fooSass from 'foo.scss';
  import barCss from 'bar.css';
  ```

**[⬆ Back to top](#table-of-contents)**

## Iterators and Generators

- Don’t use iterators. Prefer JavaScript’s higher-order functions instead of loops like `for-in` or `for-of`. eslint: [`no-iterator`](https://eslint.org/docs/rules/no-iterator.html) [`no-restricted-syntax`](https://eslint.org/docs/rules/no-restricted-syntax)

  > Why? This enforces our immutable rule. Dealing with pure functions that return values is easier to reason about than side effects.
  >
  > Use `map()` / `every()` / `filter()` / `find()` / `findIndex()` / `reduce()` / `some()` / ... to iterate over arrays, and `Object.keys()` / `Object.values()` / `Object.entries()` to produce arrays so you can iterate over objects.

  ```javascript
  const numbers = [1, 2, 3, 4, 5];

  // bad
  let sum = 0;
  for (let num of numbers) {
    sum += num;
  }
  sum === 15;

  // good
  let sum = 0;
  numbers.forEach((num) => {
    sum += num;
  });
  sum === 15;

  // best (use the functional force)
  const sum = numbers.reduce((total, num) => total + num, 0);
  sum === 15;

  // bad
  const increasedByOne = [];
  for (let i = 0; i < numbers.length; i++) {
    increasedByOne.push(numbers[i] + 1);
  }

  // good
  const increasedByOne = [];
  numbers.forEach((num) => {
    increasedByOne.push(num + 1);
  });

  // best (keeping it functional)
  const increasedByOne = numbers.map((num) => num + 1);
  ```

- Don’t use generators for now.

  > Why? They don’t transpile well to ES5.

**[⬆ Back to top](#table-of-contents)**

## Properties

- Use dot notation when accessing properties. eslint: [`dot-notation`](https://eslint.org/docs/rules/dot-notation.html)

  ```javascript
  const luke = {
    jedi: true,
    age: 28,
  };

  // bad
  const isJedi = luke['jedi'];

  // good
  const isJedi = luke.jedi;
  ```

- Use bracket notation `[]` when accessing properties with a variable.

  ```javascript
  const luke = {
    jedi: true,
    age: 28,
  };

  function getProp(prop) {
    return luke[prop];
  }

  const isJedi = getProp('jedi');
  ```

- Use exponentiation operator `**` when calculating exponentiations. eslint: [`no-restricted-properties`](https://eslint.org/docs/rules/no-restricted-properties).

  ```javascript
  // bad
  const binary = Math.pow(2, 10);

  // good
  const binary = 2 ** 10;
  ```

**[⬆ Back to top](#table-of-contents)**

## Variables

- Always use `const` or `let` to declare variables. Not doing so will result in global variables. We want to avoid polluting the global namespace. eslint: [`no-undef`](https://eslint.org/docs/rules/no-undef) [`prefer-const`](https://eslint.org/docs/rules/prefer-const)

  ```javascript
  // bad
  superPower = new SuperPower();

  // good
  const superPower = new SuperPower();
  ```

- Use one `const` or `let` declaration per variable or assignment. eslint: [`one-var`](https://eslint.org/docs/rules/one-var.html)

  > Why? It’s easier to add new variable declarations this way, and you never have to worry about swapping out a `;` for a `,` or introducing punctuation-only diffs. You can also step through each declaration with the debugger, instead of jumping through all of them at once.

  ```javascript
  // bad
  const items = getItems(),
      goSportsTeam = true,
      dragonball = 'z';

  // bad
  // (compare to above, and try to spot the mistake)
  const items = getItems(),
      goSportsTeam = true;
      dragonball = 'z';

  // good
  const items = getItems();
  const goSportsTeam = true;
  const dragonball = 'z';
  ```

- Group all your `const`s and then group all your `let`s.

  > Why? This is helpful when later on you might need to assign a variable depending on one of the previous assigned variables.

  ```javascript
  // bad
  let i, len, dragonball,
      items = getItems(),
      goSportsTeam = true;

  // bad
  let i;
  const items = getItems();
  let dragonball;
  const goSportsTeam = true;
  let len;

  // good
  const goSportsTeam = true;
  const items = getItems();
  let dragonball;
  let i;
  let length;
  ```

- Assign variables where you need them, but place them in a reasonable place.

  > Why? `let` and `const` are block scoped and not function scoped.

  ```javascript
  // bad - unnecessary function call
  function checkName(hasName) {
    const name = getName();

    if (hasName === 'test') {
      return false;
    }

    if (name === 'test') {
      this.setName('');
      return false;
    }

    return name;
  }

  // good
  function checkName(hasName) {
    if (hasName === 'test') {
      return false;
    }

    const name = getName();

    if (name === 'test') {
      this.setName('');
      return false;
    }

    return name;
  }
  ```

- Don’t chain variable assignments. eslint: [`no-multi-assign`](https://eslint.org/docs/rules/no-multi-assign)

  > Why? Chaining variable assignments creates implicit global variables.

  ```javascript
  // bad
  (function example() {
    // JavaScript interprets this as
    // let a = ( b = ( c = 1 ) );
    // The let keyword only applies to variable a; variables b and c become
    // global variables.
    let a = b = c = 1;
  }());

  console.log(a); // throws ReferenceError
  console.log(b); // 1
  console.log(c); // 1

  // good
  (function example() {
    let a = 1;
    let b = a;
    let c = a;
  }());

  console.log(a); // throws ReferenceError
  console.log(b); // throws ReferenceError
  console.log(c); // throws ReferenceError

  // the same applies for `const`
  ```

- Avoid using unary increments and decrements (`++`, `--`). eslint [`no-plusplus`](https://eslint.org/docs/rules/no-plusplus)

  > Why? Per the eslint documentation, unary increment and decrement statements are subject to automatic semicolon insertion and can cause silent errors with incrementing or decrementing values within an application. It is also more expressive to mutate your values with statements like `num += 1` instead of `num++` or `num ++`. Disallowing unary increment and decrement statements also prevents you from pre-incrementing/pre-decrementing values unintentionally which can also cause unexpected behavior in your programs.

  ```javascript
  // bad

  const array = [1, 2, 3];
  let num = 1;
  num++;
  --num;

  let sum = 0;
  let truthyCount = 0;
  for (let i = 0; i < array.length; i++) {
    let value = array[i];
    sum += value;
    if (value) {
      truthyCount++;
    }
  }

  // good

  const array = [1, 2, 3];
  let num = 1;
  num += 1;
  num -= 1;

  const sum = array.reduce((a, b) => a + b, 0);
  const truthyCount = array.filter(Boolean).length;
  ```

- Avoid linebreaks before or after `=` in an assignment. If your assignment violates [`max-len`](https://eslint.org/docs/rules/max-len.html), surround the value in parens. eslint [`operator-linebreak`](https://eslint.org/docs/rules/operator-linebreak.html).

  > Why? Linebreaks surrounding `=` can obfuscate the value of an assignment.

  ```javascript
  // bad
  const foo =
    superLongLongLongLongLongLongLongLongFunctionName();

  // bad
  const foo
    = 'superLongLongLongLongLongLongLongLongString';

  // good
  const foo = (
    superLongLongLongLongLongLongLongLongFunctionName()
  );

  // good
  const foo = 'superLongLongLongLongLongLongLongLongString';
  ```

- Disallow unused variables. eslint: [`no-unused-vars`](https://eslint.org/docs/rules/no-unused-vars)

  > Why? Variables that are declared and not used anywhere in the code are most likely an error due to incomplete refactoring. Such variables take up space in the code and can lead to confusion by readers.

  ```javascript
  // bad

  var some_unused_var = 42;

  // Write-only variables are not considered as used.
  var y = 10;
  y = 5;

  // A read for a modification of itself is not considered as used.
  var z = 0;
  z = z + 1;

  // Unused function arguments.
  function getX(x, y) {
      return x;
  }

  // good

  function getXPlusY(x, y) {
    return x + y;
  }

  var x = 1;
  var y = a + 2;

  alert(getXPlusY(x, y));

  // 'type' is ignored even if unused because it has a rest property sibling.
  // This is a form of extracting an object that omits the specified keys.
  var { type, ...coords } = data;
  // 'coords' is now the 'data' object without its 'type' property.
  ```

**[⬆ Back to top](#table-of-contents)**

## Hoisting

- `var` declarations get hoisted to the top of their closest enclosing function scope, their assignment does not. `const` and `let` declarations are blessed with a new concept called [Temporal Dead Zones (TDZ)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let#Temporal_dead_zone). It’s important to know why [typeof is no longer safe](http://es-discourse.com/t/why-typeof-is-no-longer-safe/15).

  ```javascript
  // we know this wouldn’t work (assuming there
  // is no notDefined global variable)
  function example() {
    console.log(notDefined); // => throws a ReferenceError
  }

  // creating a variable declaration after you
  // reference the variable will work due to
  // variable hoisting. Note: the assignment
  // value of `true` is not hoisted.
  function example() {
    console.log(declaredButNotAssigned); // => undefined
    var declaredButNotAssigned = true;
  }

  // the interpreter is hoisting the variable
  // declaration to the top of the scope,
  // which means our example could be rewritten as:
  function example() {
    let declaredButNotAssigned;
    console.log(declaredButNotAssigned); // => undefined
    declaredButNotAssigned = true;
  }

  // using const and let
  function example() {
    console.log(declaredButNotAssigned); // => throws a ReferenceError
    console.log(typeof declaredButNotAssigned); // => throws a ReferenceError
    const declaredButNotAssigned = true;
  }
  ```

- Anonymous function expressions hoist their variable name, but not the function assignment.

  ```javascript
  function example() {
    console.log(anonymous); // => undefined

    anonymous(); // => TypeError anonymous is not a function

    var anonymous = function () {
      console.log('anonymous function expression');
    };
  }
  ```

- Named function expressions hoist the variable name, not the function name or the function body.

  ```javascript
  function example() {
    console.log(named); // => undefined

    named(); // => TypeError named is not a function

    superPower(); // => ReferenceError superPower is not defined

    var named = function superPower() {
      console.log('Flying');
    };
  }

  // the same is true when the function name
  // is the same as the variable name.
  function example() {
    console.log(named); // => undefined

    named(); // => TypeError named is not a function

    var named = function named() {
      console.log('named');
    };
  }
  ```

- Function declarations hoist their name and the function body.

  ```javascript
  function example() {
    superPower(); // => Flying

    function superPower() {
      console.log('Flying');
    }
  }
  ```

- For more information refer to [JavaScript Scoping & Hoisting](http://www.adequatelygood.com/2010/2/JavaScript-Scoping-and-Hoisting/) by [Ben Cherry](http://www.adequatelygood.com/).

**[⬆ Back to top](#table-of-contents)**

## Comparison Operators & Equality

- Use `===` and `!==` over `==` and `!=`. eslint: [`eqeqeq`](https://eslint.org/docs/rules/eqeqeq.html)

- Conditional statements such as the `if` statement evaluate their expression using coercion with the `ToBoolean` abstract method and always follow these simple rules:

  - **Objects** evaluate to **true**
  - **Undefined** evaluates to **false**
  - **Null** evaluates to **false**
  - **Booleans** evaluate to **the value of the boolean**
  - **Numbers** evaluate to **false** if **+0, -0, or NaN**, otherwise **true**
  - **Strings** evaluate to **false** if an empty string `''`, otherwise **true**

  ```javascript
  if ([0] && []) {
    // true
    // an array (even an empty one) is an object, objects will evaluate to true
  }
  ```

- Use shortcuts for booleans, but explicit comparisons for strings and numbers.

  ```javascript
  // bad
  if (isValid === true) {
    // ...
  }

  // good
  if (isValid) {
    // ...
  }

  // bad
  if (name) {
    // ...
  }

  // good
  if (name !== '') {
    // ...
  }

  // bad
  if (collection.length) {
    // ...
  }

  // good
  if (collection.length > 0) {
    // ...
  }
  ```
  
  For more information see [Truth Equality and JavaScript](https://javascriptweblog.wordpress.com/2011/02/07/truth-equality-and-javascript/#more-2108) by Angus Croll.

- Use braces to create blocks in `case` and `default` clauses that contain lexical declarations (e.g. `let`, `const`, `function`, and `class`). eslint: [`no-case-declarations`](https://eslint.org/docs/rules/no-case-declarations.html)

  > Why? Lexical declarations are visible in the entire `switch` block but only get initialized when assigned, which only happens when its `case` is reached. This causes problems when multiple `case` clauses attempt to define the same thing.

  ```javascript
  // bad
  switch (foo) {
    case 1:
      let x = 1;
      break;
    case 2:
      const y = 2;
      break;
    case 3:
      function f() {
        // ...
      }
      break;
    default:
      class C {}
  }

  // good
  switch (foo) {
    case 1: {
      let x = 1;
      break;
    }
    case 2: {
      const y = 2;
      break;
    }
    case 3: {
      function f() {
        // ...
      }
      break;
    }
    case 4:
      bar();
      break;
    default: {
      class C {}
    }
  }
  ```

- Ternaries should not be nested and generally be single line expressions. eslint: [`no-nested-ternary`](https://eslint.org/docs/rules/no-nested-ternary.html)

  ```javascript
  // bad
  const foo = maybe1 > maybe2
    ? "bar"
    : value1 > value2 ? "baz" : null;

  // split into 2 separated ternary expressions
  const maybeNull = value1 > value2 ? 'baz' : null;

  // better
  const foo = maybe1 > maybe2
    ? 'bar'
    : maybeNull;

  // best
  const foo = maybe1 > maybe2 ? 'bar' : maybeNull;
  ```

- Avoid unneeded ternary statements. eslint: [`no-unneeded-ternary`](https://eslint.org/docs/rules/no-unneeded-ternary.html)

  ```javascript
  // bad
  const foo = a ? a : b;
  const bar = c ? true : false;
  const baz = c ? false : true;

  // good
  const foo = a || b;
  const bar = !!c;
  const baz = !c;
  ```

- When mixing operators, enclose them in parentheses. The only exception is the standard arithmetic operators: `+`, `-`, and `**` since their precedence is broadly understood. We recommend enclosing `/` and `*` in parentheses because their precedence can be ambiguous when they are mixed.
eslint: [`no-mixed-operators`](https://eslint.org/docs/rules/no-mixed-operators.html)

  > Why? This improves readability and clarifies the developer’s intention.

  ```javascript
  // bad
  const foo = a && b < 0 || c > 0 || d + 1 === 0;

  // bad
  const bar = a ** b - 5 % d;

  // bad
  // one may be confused into thinking (a || b) && c
  if (a || b && c) {
    return d;
  }

  // bad
  const bar = a + b / c * d;

  // good
  const foo = (a && b < 0) || c > 0 || (d + 1 === 0);

  // good
  const bar = a ** b - (5 % d);

  // good
  if (a || (b && c)) {
    return d;
  }

  // good
  const bar = a + (b / c) * d;
  ```

**[⬆ Back to top](#table-of-contents)**

## Blocks

- Use braces with all multiline blocks. eslint: [`nonblock-statement-body-position`](https://eslint.org/docs/rules/nonblock-statement-body-position)

  ```javascript
  // bad
  if (test)
    return false;

  // good
  if (test) return false;

  // good
  if (test) {
    return false;
  }

  // bad
  function foo() { return false; }

  // good
  function bar() {
    return false;
  }
  ```

- If you’re using multiline blocks with `if` and `else`, put `else` on the same line as your `if` block’s closing brace. eslint: [`brace-style`](https://eslint.org/docs/rules/brace-style.html)

  ```javascript
  // bad
  if (test) {
    thing1();
    thing2();
  }
  else {
    thing3();
  }

  // good
  if (test) {
    thing1();
    thing2();
  } else {
    thing3();
  }
  ```

- If an `if` block always executes a `return` statement, the subsequent `else` block is unnecessary. A `return` in an `else if` block following an `if` block that contains a `return` can be separated into multiple `if` blocks. eslint: [`no-else-return`](https://eslint.org/docs/rules/no-else-return)

  ```javascript
  // bad
  function foo() {
    if (x) {
      return x;
    } else {
      return y;
    }
  }

  // bad
  function cats() {
    if (x) {
      return x;
    } else if (y) {
      return y;
    }
  }

  // bad
  function dogs() {
    if (x) {
      return x;
    } else {
      if (y) {
        return y;
      }
    }
  }

  // good
  function foo() {
    if (x) {
      return x;
    }

    return y;
  }

  // good
  function cats() {
    if (x) {
      return x;
    }

    if (y) {
      return y;
    }
  }

  // good
  function dogs(x) {
    if (x) {
      if (z) {
        return y;
      }
    } else {
      return z;
    }
  }
  ```

**[⬆ Back to top](#table-of-contents)**

## Control Statements

- In case your control statement (`if`, `while` etc.) gets too long or exceeds the maximum line length, each (grouped) condition could be put into a new line. The logical operator should begin the line.

  > Why? Requiring operators at the beginning of the line keeps the operators aligned and follows a pattern similar to method chaining. This also improves readability by making it easier to visually follow complex logic.

  ```javascript
  // bad
  if ((foo === 123 || bar === 'abc') && doesItLookGoodWhenItBecomesThatLong() && isThisReallyHappening()) {
    thing1();
  }

  // bad
  if (foo === 123 &&
    bar === 'abc') {
    thing1();
  }

  // bad
  if (foo === 123
    && bar === 'abc') {
    thing1();
  }

  // bad
  if (
    foo === 123 &&
    bar === 'abc'
  ) {
    thing1();
  }

  // good
  if (
    foo === 123
    && bar === 'abc'
  ) {
    thing1();
  }

  // good
  if (
    (foo === 123 || bar === 'abc')
    && doesItLookGoodWhenItBecomesThatLong()
    && isThisReallyHappening()
  ) {
    thing1();
  }

  // good
  if (foo === 123 && bar === 'abc') {
    thing1();
  }
  ```

- Don't use selection operators in place of control statements.

  ```javascript
  // bad
  !isRunning && startRunning();

  // good
  if (!isRunning) {
    startRunning();
  }
  ```

**[⬆ Back to top](#table-of-contents)**

## Comments

- Use `/** ... */` for multiline comments.

  ```javascript
  // bad
  // make() returns a new element
  // based on the passed in tag name
  //
  // @param {String} tag
  // @return {Element} element
  function make(tag) {

    // ...

    return element;
  }

  // good
  /**
   * make() returns a new element
   * based on the passed-in tag name
   */
  function make(tag) {

    // ...

    return element;
  }
  ```

- Use `//` for single line comments. Place single line comments on a newline above the subject of the comment. Put an empty line before the comment unless it’s on the first line of a block.

  ```javascript
  // bad
  const active = true;  // is current tab

  // good
  // is current tab
  const active = true;

  // bad
  function getType() {
    console.log('fetching type...');
    // set the default type to 'no type'
    const type = this.type || 'no type';

    return type;
  }

  // good
  function getType() {
    console.log('fetching type...');

    // set the default type to 'no type'
    const type = this.type || 'no type';

    return type;
  }

  // also good
  function getType() {
    // set the default type to 'no type'
    const type = this.type || 'no type';

    return type;
  }
  ```

- Start all comments with a space to make it easier to read. eslint: [`spaced-comment`](https://eslint.org/docs/rules/spaced-comment)

  ```javascript
  // bad
  //is current tab
  const active = true;

  // good
  // is current tab
  const active = true;

  // bad
  /**
   *make() returns a new element
    *based on the passed-in tag name
    */
  function make(tag) {

    // ...

    return element;
  }

  // good
  /**
   * make() returns a new element
   * based on the passed-in tag name
   */
  function make(tag) {

    // ...

    return element;
  }
  ```

- Prefixing your comments with `FIXME` or `TODO` helps other developers quickly understand if you’re pointing out a problem that needs to be revisited, or if you’re suggesting a solution to the problem that needs to be implemented. These are different than regular comments because they are actionable. The actions are `FIXME: -- need to figure this out` or `TODO: -- need to implement`.

- Use `// FIXME:` to annotate problems.

  ```javascript
  class Calculator extends Abacus {
    constructor() {
      super();

      // FIXME: shouldn’t use a global here
      total = 0;
    }
  }
  ```

- Use `// TODO:` to annotate solutions to problems.

  ```javascript
  class Calculator extends Abacus {
    constructor() {
      super();

      // TODO: total should be configurable by an options param
      this.total = 0;
    }
  }
  ```

**[⬆ Back to top](#table-of-contents)**

## Whitespace

- Use soft tabs (space character) set to 2 spaces. eslint: [`indent`](https://eslint.org/docs/rules/indent.html)

  ```javascript
  // bad
  function foo() {
  ∙∙∙∙let name;
  }

  // bad
  function bar() {
  ∙let name;
  }

  // good
  function baz() {
  ∙∙let name;
  }
  ```

- Place 1 space before the leading brace. eslint: [`space-before-blocks`](https://eslint.org/docs/rules/space-before-blocks.html)

  ```javascript
  // bad
  function test(){
    console.log('test');
  }

  // good
  function test() {
    console.log('test');
  }

  // bad
  dog.set('attr',{
    age: '1 year',
    breed: 'Bernese Mountain Dog',
  });

  // good
  dog.set('attr', {
    age: '1 year',
    breed: 'Bernese Mountain Dog',
  });
  ```

- Place 1 space before the opening parenthesis in control statements (`if`, `while` etc.). Place no space between the argument list and the function name in function calls and declarations. eslint: [`keyword-spacing`](https://eslint.org/docs/rules/keyword-spacing.html)

  ```javascript
  // bad
  if(isJedi) {
    fight ();
  }

  // good
  if (isJedi) {
    fight();
  }

  // bad
  function fight () {
    console.log ('Swooosh!');
  }

  // good
  function fight() {
    console.log('Swooosh!');
  }
  ```

- Set off operators with spaces. eslint: [`space-infix-ops`](https://eslint.org/docs/rules/space-infix-ops.html)

  ```javascript
  // bad
  const x=y+5;

  // good
  const x = y + 5;
  ```

- End files with a single newline character. eslint: [`eol-last`](https://github.com/eslint/eslint/blob/master/docs/rules/eol-last.md)

  ```javascript
  // bad
  import { es6 } from './AirbnbStyleGuide';
  // ...
  export default es6;
  ```

  ```javascript
  // bad
  import { es6 } from './AirbnbStyleGuide';
  // ...
  export default es6;↵
  ↵
  ```

  ```javascript
  // good
  import { es6 } from './AirbnbStyleGuide';
  // ...
  export default es6;↵
  ```

- Use indentation when making long method chains (more than 2 method chains). Use a leading dot, which
  emphasizes that the line is a method call, not a new statement. eslint: [`newline-per-chained-call`](https://eslint.org/docs/rules/newline-per-chained-call) [`no-whitespace-before-property`](https://eslint.org/docs/rules/no-whitespace-before-property)

  ```javascript
  // bad
  $('#items').find('.selected').highlight().end().find('.open').updateCount();

  // bad
  $('#items').
    find('.selected').
      highlight().
      end().
    find('.open').
      updateCount();

  // good
  $('#items')
    .find('.selected')
      .highlight()
      .end()
    .find('.open')
      .updateCount();

  // bad
  const leds = stage.selectAll('.led').data(data).enter().append('svg:svg').classed('led', true)
      .attr('width', (radius + margin) * 2).append('svg:g')
      .attr('transform', `translate(${radius + margin},${radius + margin})`)
      .call(tron.led);

  // good
  const leds = stage.selectAll('.led')
      .data(data)
    .enter().append('svg:svg')
      .classed('led', true)
      .attr('width', (radius + margin) * 2)
    .append('svg:g')
      .attr('transform', `translate(${radius + margin},${radius + margin})`)
      .call(tron.led);

  // good
  const leds = stage.selectAll('.led').data(data);
  ```

- Leave a blank line after blocks and before the next statement.

  ```javascript
  // bad
  if (foo) {
    return bar;
  }
  return baz;

  // good
  if (foo) {
    return bar;
  }

  return baz;

  // bad
  const obj = {
    foo() {
    },
    bar() {
    },
  };
  return obj;

  // good
  const obj = {
    foo() {
    },

    bar() {
    },
  };

  return obj;

  // bad
  const arr = [
    function foo() {
    },
    function bar() {
    },
  ];
  return arr;

  // good
  const arr = [
    function foo() {
    },

    function bar() {
    },
  ];

  return arr;
  ```

- Do not pad your blocks with blank lines. eslint: [`padded-blocks`](https://eslint.org/docs/rules/padded-blocks.html)

  ```javascript
  // bad
  function bar() {

    console.log(foo);

  }

  // bad
  if (baz) {

    console.log(qux);
  } else {
    console.log(foo);

  }

  // bad
  class Foo {

    constructor(bar) {
      this.bar = bar;
    }
  }

  // good
  function bar() {
    console.log(foo);
  }

  // good
  if (baz) {
    console.log(qux);
  } else {
    console.log(foo);
  }
  ```

- Do not use multiple blank lines to pad your code. eslint: [`no-multiple-empty-lines`](https://eslint.org/docs/rules/no-multiple-empty-lines)

  <!-- markdownlint-disable MD012 -->
  ```javascript
  // bad
  class Person {
    constructor(fullName, email, birthday) {
      this.fullName = fullName;


      this.email = email;


      this.setAge(birthday);
    }


    setAge(birthday) {
      const today = new Date();


      const age = this.getAge(today, birthday);


      this.age = age;
    }


    getAge(today, birthday) {
      // ..
    }
  }

  // good
  class Person {
    constructor(fullName, email, birthday) {
      this.fullName = fullName;
      this.email = email;
      this.setAge(birthday);
    }

    setAge(birthday) {
      const today = new Date();
      const age = getAge(today, birthday);
      this.age = age;
    }

    getAge(today, birthday) {
      // ..
    }
  }
  ```

- Do not add spaces inside parentheses. eslint: [`space-in-parens`](https://eslint.org/docs/rules/space-in-parens.html)

  ```javascript
  // bad
  function bar( foo ) {
    return foo;
  }

  // good
  function bar(foo) {
    return foo;
  }

  // bad
  if ( foo ) {
    console.log(foo);
  }

  // good
  if (foo) {
    console.log(foo);
  }
  ```

- Do not add spaces inside brackets. eslint: [`array-bracket-spacing`](https://eslint.org/docs/rules/array-bracket-spacing.html)

  ```javascript
  // bad
  const foo = [ 1, 2, 3 ];
  console.log(foo[ 0 ]);

  // good
  const foo = [1, 2, 3];
  console.log(foo[0]);
  ```

- Add spaces inside curly braces. eslint: [`object-curly-spacing`](https://eslint.org/docs/rules/object-curly-spacing.html)

  ```javascript
  // bad
  const foo = {clark: 'kent'};

  // good
  const foo = { clark: 'kent' };
  ```

- Require consistent spacing inside an open block token and the next token on the same line. This rule also enforces consistent spacing inside a close block token and previous token on the same line. eslint: [`block-spacing`](https://eslint.org/docs/rules/block-spacing)

  ```javascript
  // bad
  function foo() {return true;}
  if (foo) { bar = 0;}

  // good
  function foo() { return true; }
  if (foo) { bar = 0; }
  ```

- Avoid spaces before commas and require a space after commas. eslint: [`comma-spacing`](https://eslint.org/docs/rules/comma-spacing)

  ```javascript
  // bad
  var foo = 1,bar = 2;
  var arr = [1 , 2];

  // good
  var foo = 1, bar = 2;
  var arr = [1, 2];
  ```

- Enforce spacing inside of computed property brackets. eslint: [`computed-property-spacing`](https://eslint.org/docs/rules/computed-property-spacing)

  ```javascript
  // bad
  obj[foo ]
  obj[ 'foo']
  var x = {[ b ]: a}
  obj[foo[ bar ]]

  // good
  obj[foo]
  obj['foo']
  var x = { [b]: a }
  obj[foo[bar]]
  ```

- Avoid spaces between functions and their invocations. eslint: [`func-call-spacing`](https://eslint.org/docs/rules/func-call-spacing)

  ```javascript
  // bad
  func ();

  func
  ();

  // good
  func();
  ```

- Enforce spacing between keys and values in object literal properties. eslint: [`key-spacing`](https://eslint.org/docs/rules/key-spacing)

  ```javascript
  // bad
  var obj = { "foo" : 42 };
  var obj2 = { "foo":42 };

  // good
  var obj = { "foo": 42 };
  ```

- Avoid trailing spaces at the end of lines. eslint: [`no-trailing-spaces`](https://eslint.org/docs/rules/no-trailing-spaces)

- Avoid multiple empty lines, only allow one newline at the end of files, and avoid a newline at the beginning of files. eslint: [`no-multiple-empty-lines`](https://eslint.org/docs/rules/no-multiple-empty-lines)

  <!-- markdownlint-disable MD012 -->
  ```javascript
  // bad - multiple empty lines
  var x = 1;


  var y = 2;

  // bad - 2+ newlines at end of file
  var x = 1;
  var y = 2;


  // bad - 1+ newline(s) at beginning of file

  var x = 1;
  var y = 2;

  // good
  var x = 1;
  var y = 2;

  ```
  <!-- markdownlint-enable MD012 -->

**[⬆ Back to top](#table-of-contents)**

## Commas

- Leading commas: **Nope.** eslint: [`comma-style`](https://eslint.org/docs/rules/comma-style.html)

  ```javascript
  // bad
  const story = [
      once
    , upon
    , aTime
  ];

  // good
  const story = [
    once,
    upon,
    aTime,
  ];

  // bad
  const hero = {
      firstName: 'Ada'
    , lastName: 'Lovelace'
    , birthYear: 1815
    , superPower: 'computers'
  };

  // good
  const hero = {
    firstName: 'Ada',
    lastName: 'Lovelace',
    birthYear: 1815,
    superPower: 'computers',
  };
  ```

- Additional trailing comma: **Yup.** eslint: [`comma-dangle`](https://eslint.org/docs/rules/comma-dangle.html)

  > Why? This leads to cleaner git diffs. Also, transpilers like Babel will remove the additional trailing comma in the transpiled code which means you don’t have to worry about the [trailing comma problem](https://github.com/airbnb/javascript/blob/es5-deprecated/es5/README.md#commas) in legacy browsers.

  ```diff
  // bad - git diff without trailing comma
  const hero = {
        firstName: 'Florence',
  -    lastName: 'Nightingale'
  +    lastName: 'Nightingale',
  +    inventorOf: ['coxcomb chart', 'modern nursing']
  };

  // good - git diff with trailing comma
  const hero = {
        firstName: 'Florence',
        lastName: 'Nightingale',
  +    inventorOf: ['coxcomb chart', 'modern nursing'],
  };
  ```

  ```javascript
  // bad
  const hero = {
    firstName: 'Dana',
    lastName: 'Scully'
  };

  const heroes = [
    'Batman',
    'Superman'
  ];

  // good
  const hero = {
    firstName: 'Dana',
    lastName: 'Scully',
  };

  const heroes = [
    'Batman',
    'Superman',
  ];

  // bad
  function createHero(
    firstName,
    lastName,
    inventorOf
  ) {
    // does nothing
  }

  // good
  function createHero(
    firstName,
    lastName,
    inventorOf,
  ) {
    // does nothing
  }

  // good (note that a comma must not appear after a "rest" element)
  function createHero(
    firstName,
    lastName,
    inventorOf,
    ...heroArgs
  ) {
    // does nothing
  }

  // bad
  createHero(
    firstName,
    lastName,
    inventorOf
  );

  // good
  createHero(
    firstName,
    lastName,
    inventorOf,
  );

  // good (note that a comma must not appear after a "rest" element)
  createHero(
    firstName,
    lastName,
    inventorOf,
    ...heroArgs
  );
  ```

**[⬆ Back to top](#table-of-contents)**

## Semicolons

- **Yup.** eslint: [`semi`](https://eslint.org/docs/rules/semi.html)

  > Why? When JavaScript encounters a line break without a semicolon, it uses a set of rules called [Automatic Semicolon Insertion](https://tc39.github.io/ecma262/#sec-automatic-semicolon-insertion) to determine whether or not it should regard that line break as the end of a statement, and (as the name implies) place a semicolon into your code before the line break if it thinks so. ASI contains a few eccentric behaviors, though, and your code will break if JavaScript misinterprets your line break. These rules will become more complicated as new features become a part of JavaScript. Explicitly terminating your statements and configuring your linter to catch missing semicolons will help prevent you from encountering issues.

  ```javascript
  // bad - raises exception
  const luke = {}
  const leia = {}
  [luke, leia].forEach((jedi) => jedi.father = 'vader')

  // bad - raises exception
  const reaction = "No! That’s impossible!"
  (async function meanwhileOnTheFalcon() {
    // handle `leia`, `lando`, `chewie`, `r2`, `c3p0`
    // ...
  }())

  // bad - returns `undefined` instead of the value on the next line - always happens when `return` is on a line by itself because of ASI!
  function foo() {
    return
      'search your feelings, you know it to be foo'
  }

  // good
  const luke = {};
  const leia = {};
  [luke, leia].forEach((jedi) => {
    jedi.father = 'vader';
  });

  // good
  const reaction = "No! That’s impossible!";
  (async function meanwhileOnTheFalcon() {
    // handle `leia`, `lando`, `chewie`, `r2`, `c3p0`
    // ...
  }());

  // good
  function foo() {
    return 'search your feelings, you know it to be foo';
  }
  ```

  [Read more](https://stackoverflow.com/questions/7365172/semicolon-before-self-invoking-function/7365214#7365214).

**[⬆ Back to top](#table-of-contents)**

## Type Casting & Coercion

- Perform type coercion at the beginning of the statement.

- Strings: eslint: [`no-new-wrappers`](https://eslint.org/docs/rules/no-new-wrappers)

  ```javascript
  // => this.reviewScore = 9;

  // bad
  const totalScore = new String(this.reviewScore); // typeof totalScore is "object" not "string"

  // bad
  const totalScore = this.reviewScore + ''; // invokes this.reviewScore.valueOf()

  // bad
  const totalScore = this.reviewScore.toString(); // isn’t guaranteed to return a string

  // good
  const totalScore = String(this.reviewScore);
  ```

- Numbers: Use `Number` for type casting and `parseInt` always with a radix for parsing strings. eslint: [`radix`](https://eslint.org/docs/rules/radix) [`no-new-wrappers`](https://eslint.org/docs/rules/no-new-wrappers)

  ```javascript
  const inputValue = '4';

  // bad
  const val = new Number(inputValue);

  // bad
  const val = +inputValue;

  // bad
  const val = inputValue >> 0;

  // bad
  const val = parseInt(inputValue);

  // good
  const val = Number(inputValue);

  // good
  const val = parseInt(inputValue, 10);
  ```

- If for whatever reason you are doing something wild and `parseInt` is your bottleneck and need to use Bitshift for [performance reasons](https://jsperf.com/coercion-vs-casting/3), leave a comment explaining why and what you’re doing.

  ```javascript
  // good
  /**
   * parseInt was the reason my code was slow.
   * Bitshifting the String to coerce it to a
   * Number made it a lot faster.
   */
  const val = inputValue >> 0;
  ```

- **Note:** Be careful when using bitshift operations. Numbers are represented as [64-bit values](https://es5.github.io/#x4.3.19), but bitshift operations always return a 32-bit integer ([source](https://es5.github.io/#x11.7)). Bitshift can lead to unexpected behavior for integer values larger than 32 bits. [Discussion](https://github.com/airbnb/javascript/issues/109). Largest signed 32-bit Int is 2,147,483,647:

  ```javascript
  2147483647 >> 0; // => 2147483647
  2147483648 >> 0; // => -2147483648
  2147483649 >> 0; // => -2147483647
  ```

- Booleans: eslint: [`no-new-wrappers`](https://eslint.org/docs/rules/no-new-wrappers)

  ```javascript
  const age = 0;

  // bad
  const hasAge = new Boolean(age);

  // good
  const hasAge = Boolean(age);

  // best
  const hasAge = !!age;
  ```

**[⬆ Back to top](#table-of-contents)**

## Naming Conventions

- Avoid single letter names. Be descriptive with your naming. eslint: [`id-length`](https://eslint.org/docs/rules/id-length)

  ```javascript
  // bad
  function q() {
    // ...
  }

  // good
  function query() {
    // ...
  }
  ```

- Use camelCase when naming objects, functions, and instances. eslint: [`camelcase`](https://eslint.org/docs/rules/camelcase.html)

  ```javascript
  // bad
  const OBJEcttsssss = {};
  const this_is_my_object = {};
  function c() {}

  // good
  const thisIsMyObject = {};
  function thisIsMyFunction() {}
  ```

- Use PascalCase only when naming constructors or classes. eslint: [`new-cap`](https://eslint.org/docs/rules/new-cap.html)

  ```javascript
  // bad
  function user(options) {
    this.name = options.name;
  }

  const bad = new user({
    name: 'nope',
  });

  // good
  class User {
    constructor(options) {
      this.name = options.name;
    }
  }

  const good = new User({
    name: 'yup',
  });
  ```

- Do not use trailing or leading underscores. eslint: [`no-underscore-dangle`](https://eslint.org/docs/rules/no-underscore-dangle.html)

  > Why? JavaScript does not have the concept of privacy in terms of properties or methods. Although a leading underscore is a common convention to mean “private”, in fact, these properties are fully public, and as such, are part of your public API contract. This convention might lead developers to wrongly think that a change won’t count as breaking, or that tests aren’t needed. tl;dr: if you want something to be “private”, it must not be observably present.

  ```javascript
  // bad
  this.__firstName__ = 'Panda';
  this.firstName_ = 'Panda';
  this._firstName = 'Panda';

  // good
  this.firstName = 'Panda';

  // good, in environments where WeakMaps are available
  // see https://kangax.github.io/compat-table/es6/#test-WeakMap
  const firstNames = new WeakMap();
  firstNames.set(this, 'Panda');
  ```

- Don’t save references to `this`. Use arrow functions or [Function#bind](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/bind).

  ```javascript
  // bad
  function foo() {
    const self = this;
    return function () {
      console.log(self);
    };
  }

  // bad
  function foo() {
    const that = this;
    return function () {
      console.log(that);
    };
  }

  // good
  function foo() {
    return () => {
      console.log(this);
    };
  }
  ```

- A base filename should exactly match the name of its default export.

  ```javascript
  // file 1 contents
  class CheckBox {
    // ...
  }
  export default CheckBox;

  // file 2 contents
  export default function fortyTwo() { return 42; }

  // file 3 contents
  export default function insideDirectory() {}

  // in some other file
  // bad
  import CheckBox from './checkBox'; // PascalCase import/export, camelCase filename
  import FortyTwo from './FortyTwo'; // PascalCase import/filename, camelCase export
  import InsideDirectory from './InsideDirectory'; // PascalCase import/filename, camelCase export

  // bad
  import CheckBox from './check_box'; // PascalCase import/export, snake_case filename
  import forty_two from './forty_two'; // snake_case import/filename, camelCase export
  import inside_directory from './inside_directory'; // snake_case import, camelCase export
  import index from './inside_directory/index'; // requiring the index file explicitly
  import insideDirectory from './insideDirectory/index'; // requiring the index file explicitly

  // good
  import CheckBox from './CheckBox'; // PascalCase export/import/filename
  import fortyTwo from './fortyTwo'; // camelCase export/import/filename
  import insideDirectory from './insideDirectory'; // camelCase export/import/directory name/implicit "index"
  // ^ supports both insideDirectory.js and insideDirectory/index.js
  ```

- Use camelCase when you export-default a function. Your filename should be identical to your function’s name.

  ```javascript
  function makeStyleGuide() {
    // ...
  }

  export default makeStyleGuide;
  ```

- Use PascalCase when you export a constructor / class / singleton / function library / bare object.

  ```javascript
  const AirbnbStyleGuide = {
    es6: {
    },
  };

  export default AirbnbStyleGuide;
  ```

- Acronyms and initialisms should always be all uppercased, or all lowercased.

  > Why? Names are for readability, not to appease a computer algorithm.

  ```javascript
  // bad
  import SmsContainer from './containers/SmsContainer';

  // bad
  const HttpRequests = [
    // ...
  ];

  // good
  import SMSContainer from './containers/SMSContainer';

  // good
  const HTTPRequests = [
    // ...
  ];

  // also good
  const httpRequests = [
    // ...
  ];

  // best
  import TextMessageContainer from './containers/TextMessageContainer';

  // best
  const requests = [
    // ...
  ];
  ```

- You may optionally uppercase a constant only if it (1) is exported, (2) is a `const` (it can not be reassigned), and (3) the programmer can trust it (and its nested properties) to never change.

  > Why? This is an additional tool to assist in situations where the programmer would be unsure if a variable might ever change. UPPERCASE_VARIABLES are letting the programmer know that they can trust the variable (and its properties) not to change.
  - What about all `const` variables? - This is unnecessary, so uppercasing should not be used for constants within a file. It should be used for exported constants however.
  - What about exported objects? - Uppercase at the top level of export (e.g. `EXPORTED_OBJECT.key`) and maintain that all nested properties do not change.

  ```javascript
  // bad
  const PRIVATE_VARIABLE = 'should not be unnecessarily uppercased within a file';

  // bad
  export const THING_TO_BE_CHANGED = 'should obviously not be uppercased';

  // bad
  export let REASSIGNABLE_VARIABLE = 'do not use let with uppercase variables';

  // ---

  // allowed but does not supply semantic value
  export const apiKey = 'SOMEKEY';

  // better in most cases
  export const API_KEY = 'SOMEKEY';

  // ---

  // bad - unnecessarily uppercases key while adding no semantic value
  export const MAPPING = {
    KEY: 'value'
  };

  // good
  export const MAPPING = {
    key: 'value'
  };
  ```

**[⬆ Back to top](#table-of-contents)**

## Accessors

- Accessor functions for properties are not required.

- Do not use JavaScript getters/setters as they cause unexpected side effects and are harder to test, maintain, and reason about. Instead, if you do make accessor functions, use `getVal()` and `setVal('hello')`.

  ```javascript
  // bad
  class Dragon {
    get age() {
      // ...
    }

    set age(value) {
      // ...
    }
  }

  // good
  class Dragon {
    getAge() {
      // ...
    }

    setAge(value) {
      // ...
    }
  }
  ```

- If the property/method is a `boolean`, use `isVal()` or `hasVal()`.

  ```javascript
  // bad
  if (!dragon.age()) {
    return false;
  }

  // good
  if (!dragon.hasAge()) {
    return false;
  }
  ```

- It’s okay to create `get()` and `set()` functions, but be consistent.

  ```javascript
  class Jedi {
    constructor(options = {}) {
      const lightsaber = options.lightsaber || 'blue';
      this.set('lightsaber', lightsaber);
    }

    set(key, val) {
      this[key] = val;
    }

    get(key) {
      return this[key];
    }
  }
  ```

**[⬆ Back to top](#table-of-contents)**

## Events

- When attaching data payloads to events (whether DOM events or something more proprietary like Backbone events), pass an object literal (also known as a "hash") instead of a raw value. This allows a subsequent contributor to add more data to the event payload without finding and updating every handler for the event. For example, instead of:

  ```javascript
  // bad
  $(this).trigger('listingUpdated', listing.id);

  // ...

  $(this).on('listingUpdated', (e, listingID) => {
    // do something with listingID
  });
  ```

  prefer:

  ```javascript
  // good
  $(this).trigger('listingUpdated', { listingID: listing.id });

  // ...

  $(this).on('listingUpdated', (e, data) => {
    // do something with data.listingID
  });
  ```

**[⬆ Back to top](#table-of-contents)**

## jQuery

- Prefix jQuery object variables with a `$`.

  ```javascript
  // bad
  const sidebar = $('.sidebar');

  // good
  const $sidebar = $('.sidebar');

  // good
  const $sidebarBtn = $('.sidebar-btn');
  ```

- Cache jQuery lookups.

  ```javascript
  // bad
  function setSidebar() {
    $('.sidebar').hide();

    // ...

    $('.sidebar').css({
      'background-color': 'pink',
    });
  }

  // good
  function setSidebar() {
    const $sidebar = $('.sidebar');
    $sidebar.hide();

    // ...

    $sidebar.css({
      'background-color': 'pink',
    });
  }
  ```

- For DOM queries use Cascading `$('.sidebar ul')` or parent > child `$('.sidebar > ul')`. [jsPerf](http://jsperf.com/jquery-find-vs-context-sel/16)

- Use `find` with scoped jQuery object queries.

  ```javascript
  // bad
  $('ul', '.sidebar').hide();

  // bad
  $('.sidebar').find('ul').hide();

  // good
  $('.sidebar ul').hide();

  // good
  $('.sidebar > ul').hide();

  // good
  $sidebar.find('ul').hide();
  ```

**[⬆ Back to top](#table-of-contents)**

## Standard Library

The [Standard Library](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects)
contains utilities that are functionally broken but remain for legacy reasons.

- Use `Number.isNaN` instead of global `isNaN`.
  eslint: [`no-restricted-globals`](https://eslint.org/docs/rules/no-restricted-globals)

  > Why? The global `isNaN` coerces non-numbers to numbers, returning true for anything that coerces to NaN.
  > If this behavior is desired, make it explicit.

  ```javascript
  // bad
  isNaN('1.2'); // false
  isNaN('1.2.3'); // true

  // good
  Number.isNaN('1.2.3'); // false
  Number.isNaN(Number('1.2.3')); // true
  ```

- Use `Number.isFinite` instead of global `isFinite`.
  eslint: [`no-restricted-globals`](https://eslint.org/docs/rules/no-restricted-globals)

  > Why? The global `isFinite` coerces non-numbers to numbers, returning true for anything that coerces to a finite number.
  > If this behavior is desired, make it explicit.

  ```javascript
  // bad
  isFinite('2e3'); // true

  // good
  Number.isFinite('2e3'); // false
  Number.isFinite(parseInt('2e3', 10)); // true
  ```

**[⬆ Back to top](#table-of-contents)**

## Testing

- **Yup.**

  ```javascript
  function foo() {
    return true;
  }
  ```

- **No, but seriously**:
  - Whichever testing framework you use, you should be writing tests!
  - Strive to write many small pure functions, and minimize where mutations occur.
  - Be cautious about stubs and mocks - they can make your tests more brittle.
  - We primarily use [`jest`](https://www.npmjs.com/package/jest).
  - 100% test coverage is a good goal to strive for, even if it’s not always practical to reach it.
  - Whenever you fix a bug, _write a regression test_. A bug fixed without a regression test is almost certainly going to break again in the future.
- Never use `alert()`. Only use `console.log()`.

**[⬆ Back to top](#table-of-contents)**

## JavaScript methodology

- When creating a complex series of functions, design your functions by first
  writing out in short sentences what each function's purpose is. This may take
  a little extra time, but will serve to help you gather all of your thoughts
  into a more coherent form in code and also serves as documentation.
- Early returns promote code readability with negligible performance difference

  ```javascript
  // Bad:
  function returnLate( foo ) {
    var ret;

    if ( foo ) {
      ret = "foo";
    } else {
      ret = "quux";
    }
    return ret;
  }

  // Good:
  function returnEarly( foo ) {
    if ( foo ) {
      return "foo";
    }
    return "quux";
  }
  ```
**[⬆ Back to top](#table-of-contents)**

## JavaScript tools

- [MDN JavaScript Knowledgebase](https://developer.mozilla.org/en-US/docs/Web/JavaScript):
  Reference functions from here to learn proper use and browser support
- Libraries and frameworks we use
  - [React](https://reactjs.org/)
  - [Vue](https://vuejs.org/)
  - [jQuery](https://jquery.com/)
  - [Parcel](https://parceljs.org/)

## JavaScript syntax

- Limit JavaScript files width to 80 characters
- It is considered good practice to use the type-safe equality operators `===` 
  and `!==` instead of their regular counterparts `==` and `!=`.

  > Why? The reason for this is that == and != do type coercion which follows the rather obscure Abstract Equality Comparison Algorithm. For instance, the following statements are all considered true:
  >  
  >  `([] == false) ([] == ![]) (3 == "03")`
  >
  > If one of those occurs in an innocent-looking statement such as a == b the actual problem is very difficult to spot.
- Naming convention for variables, functions, and classes should be meaningful 
  and thoughtful.

  ```javascript
  // Example of code with poor names

  function q(s) {
    return document.querySelectorAll(s);
  }
  var i,a=[],els=q("#foo");
  for(i=0;i<els.length;i++){a.push(els[i]);}
  ```


  ```javascript
  `dog` is a string

  `dogs` is an array of `dog` strings

  functionNamesLikeThis; // camelCase
  variableNamesLikeThis; // camelCase
  ConstructorNamesLikeThis; // Pascal Case
  EnumNamesLikeThis; // Pascal Case
  methodNamesLikeThis; //camelCase
  SYMBOLIC_CONSTANTS_LIKE_THIS; // upper case spaced with underscores
  ```

**[⬆ Back to top](#table-of-contents)**

# React

- Use pure functions over classes (`React.createClass`). React now has [hooks](https://reactjs.org/docs/hooks-intro.html) for state and refs so classes are no longer necessary.
- JavaScript files which use JSX should end with `.jsx` so that it's easy to 
  differentiate JavaScript that's not dependant on importing a particular 
  library like React.
- Use PascalCase for filenames. E.g., ReservationCard.jsx.
- If a function requires no type rules/testing, it can be written without a 
  namespace and short form return e.g. 

  ```jsx
  /* Avoid */
  /* Welcome.js */
  import React from 'react'

  const Welcome = () => {
    return (
      <div>
        <header>
          <h1>Welcome</h1>
          <h2>Our products are simply amazing.</h2>
          <p>
            Here is some fluffy text to get in your way more before we allow you
            to get to what you are actually looking for!
          </p>
        </header>
      </div>
    )
  }

  export default Welcome

  /* Good example */
  /* Welcome.js */
  import React from 'react'

  export default () => (
    <div>
      <header>
        <h1>Welcome</h1>
        <h2>Our products are simply amazing.</h2>
        <p>
          Here is some fluffy text to get in your way more before we allow you to
          get to what you are actually looking for!
        </p>
      </header>
    </div>
  )
  ```
  
- Only include one React component per file. Multiple pure functions are 
  allowed in a single component file.
- Always use JSX syntax.
- **Extensions**: Use `.jsx` extension for React components. eslint: [`react/jsx-filename-extension`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/jsx-filename-extension.md)
- **Filename**: Use PascalCase for filenames. E.g., `ReservationCard.jsx`.
- **Reference Naming**: Use PascalCase for React components and camelCase for 
  their instances. eslint: [`react/jsx-pascal-case`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/jsx-pascal-case.md)

  ```jsx
  // bad
  import reservationCard from './ReservationCard';

  // good
  import ReservationCard from './ReservationCard';

  // bad
  const ReservationItem = <ReservationCard />;

  // good
  const reservationItem = <ReservationCard />;
  ```

- **Component Naming**: Use the filename as the component name. For example, 
  `ReservationCard.jsx` should have a reference name of `ReservationCard`. 
  However, for root components of a directory, use `index.jsx` as the filename 
  and use the directory name as the component name:

  ```jsx
  // bad
  import Footer from './Footer/Footer';

  // bad
  import Footer from './Footer/index';

  // good
  import Footer from './Footer';
  ```

- **Higher-order Component Naming**: Use a composite of the higher-order 
  component’s name and the passed-in component’s name as the `displayName` 
  on the generated component. For example, the higher-order component 
  `withFoo()`, when passed a component `Bar` should produce a component with a 
  `displayName` of `withFoo(Bar)`. 
  [More about Higher-order Components](https://reactjs.org/docs/higher-order-components.html)

  > Why? A component’s `displayName` may be used by developer tools or in error messages, and having a value that clearly expresses this relationship helps people understand what is happening.

  ```jsx
  // bad
  export default function withFoo(WrappedComponent) {
    return function WithFoo(props) {
      return <WrappedComponent {...props} foo />;
    }
  }

  // good
  export default function withFoo(WrappedComponent) {
    function WithFoo(props) {
      return <WrappedComponent {...props} foo />;
    }

    const wrappedComponentName = WrappedComponent.displayName
      || WrappedComponent.name
      || 'Component';

    WithFoo.displayName = `withFoo(${wrappedComponentName})`;
    return WithFoo;
  }
  ```

- **Props Naming**: Avoid using DOM component prop names for different purposes.

  > Why? People expect props like `style` and `className` to mean one specific 
  thing. Varying this API for a subset of your app makes the code less readable 
  and less maintainable, and may cause bugs.

  ```jsx
  // bad
  <MyComponent style="fancy" />

  // bad
  <MyComponent className="fancy" />

  // good
  <MyComponent variant="fancy" />
  ```

**[⬆ Back to top](#table-of-contents)**

## Alignment

- Follow these alignment styles for JSX syntax. eslint: 
  [`react/jsx-closing-bracket-location`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/jsx-closing-bracket-location.md) [`react/jsx-closing-tag-location`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/jsx-closing-tag-location.md)

  ```jsx
  // bad
  <Foo superLongParam="bar"
        anotherSuperLongParam="baz" />

  // good
  <Foo
    superLongParam="bar"
    anotherSuperLongParam="baz"
  />

  // if props fit in one line then keep it on the same line
  <Foo bar="bar" />

  // children get indented normally
  <Foo
    superLongParam="bar"
    anotherSuperLongParam="baz"
  >
    <Quux />
  </Foo>

  // bad
  {showButton &&
    <Button />
  }

  // bad
  {
    showButton &&
      <Button />
  }

  // good
  {showButton && (
    <Button />
  )}

  // good
  {showButton && <Button />}
  ```

**[⬆ Back to top](#table-of-contents)**

## Quotes

- Always use double quotes (`"`) for JSX attributes, but single quotes (`'`) 
  for all other JS. eslint: 
  [`jsx-quotes`](https://eslint.org/docs/rules/jsx-quotes)

  > Why? Regular HTML attributes also typically use double quotes instead of 
  single, so JSX attributes mirror this convention.

  ```jsx
  // bad
  <Foo bar='bar' />

  // good
  <Foo bar="bar" />

  // bad
  <Foo style={{ left: "20px" }} />

  // good
  <Foo style={{ left: '20px' }} />
  ```
**[⬆ Back to top](#table-of-contents)**

## Spacing

- Always include a single space in your self-closing tag. eslint: 
  [`no-multi-spaces`](https://eslint.org/docs/rules/no-multi-spaces), [`react/jsx-tag-spacing`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/jsx-tag-spacing.md)

  ```jsx
  // bad
  <Foo/>

  // very bad
  <Foo                 />

  // bad
  <Foo
    />

  // good
  <Foo />
  ```

- Do not pad JSX curly braces with spaces. eslint: 
  [`react/jsx-curly-spacing`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/jsx-curly-spacing.md)

  ```jsx
  // bad
  <Foo bar={ baz } />

  // good
  <Foo bar={baz} />
  ```
**[⬆ Back to top](#table-of-contents)**

## Props

- Always use camelCase for prop names.

  ```jsx
  // bad
  <Foo
    UserName="hello"
    phone_number={12345678}
  />

  // good
  <Foo
    userName="hello"
    phoneNumber={12345678}
  />
  ```

- Omit the value of the prop when it is explicitly `true`. eslint: [`react/jsx-boolean-value`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/jsx-boolean-value.md)

  ```jsx
  // bad
  <Foo
    hidden={true}
  />

  // good
  <Foo
    hidden
  />

  // good
  <Foo hidden />
  ```

- Always include an `alt` prop on `<img>` tags. If the image is presentational, `alt` can be an empty string or the `<img>` must have `role="presentation"`. eslint: [`jsx-a11y/alt-text`](https://github.com/evcohen/eslint-plugin-jsx-a11y/blob/master/docs/rules/alt-text.md)

  ```jsx
  // bad
  <img src="hello.jpg" />

  // good
  <img src="hello.jpg" alt="Me waving hello" />

  // good
  <img src="hello.jpg" alt="" />

  // good
  <img src="hello.jpg" role="presentation" />
  ```

- Do not use words like "image", "photo", or "picture" in `<img>` `alt` props. eslint: [`jsx-a11y/img-redundant-alt`](https://github.com/evcohen/eslint-plugin-jsx-a11y/blob/master/docs/rules/img-redundant-alt.md)

  > Why? Screenreaders already announce `img` elements as images, so there is no need to include this information in the alt text.

  ```jsx
  // bad
  <img src="hello.jpg" alt="Picture of me waving hello" />

  // good
  <img src="hello.jpg" alt="Me waving hello" />
  ```

- Use only valid, non-abstract [ARIA roles](https://www.w3.org/TR/wai-aria/#usage_intro). eslint: [`jsx-a11y/aria-role`](https://github.com/evcohen/eslint-plugin-jsx-a11y/blob/master/docs/rules/aria-role.md)

  ```jsx
  // bad - not an ARIA role
  <div role="datepicker" />

  // bad - abstract ARIA role
  <div role="range" />

  // good
  <div role="button" />
  ```

- Do not use `accessKey` on elements. eslint: [`jsx-a11y/no-access-key`](https://github.com/evcohen/eslint-plugin-jsx-a11y/blob/master/docs/rules/no-access-key.md)

  > Why? Inconsistencies between keyboard shortcuts and keyboard commands used by people using screenreaders and keyboards complicate accessibility.

  ```jsx
  // bad
  <div accessKey="h" />

  // good
  <div />
  ```

- Avoid using an array index as `key` prop, prefer a stable ID. eslint: [`react/no-array-index-key`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/no-array-index-key.md)

  > Why? Not using a stable ID [is an anti-pattern](https://medium.com/@robinpokorny/index-as-a-key-is-an-anti-pattern-e0349aece318) because it can negatively impact performance and cause issues with component state.

  We don’t recommend using indexes for keys if the order of items may change.

  ```jsx
  // bad
  {todos.map((todo, index) =>
    <Todo
      {...todo}
      key={index}
    />
  )}

  // good
  {todos.map(todo => (
    <Todo
      {...todo}
      key={todo.id}
    />
  ))}
  ```

- Always define explicit `defaultProps` for all non-required props.

  > Why? propTypes are a form of documentation, and providing defaultProps means the reader of your code doesn’t have to assume as much. In addition, it can mean that your code can omit certain type checks.

  ```jsx
  // bad
  import PropTypes from 'prop-types'
  const SFC = ({ foo, bar, children }) => {
    return (
      <div>
        {foo}
        {bar}
        {children}
      </div>
    )
  }
  SFC.propTypes = {
    foo: PropTypes.number.isRequired,
    bar: PropTypes.string,
    children: PropTypes.node,
  }

  // good
  import PropTypes from 'prop-types'

  const SpicyComponent = ({ foo, bar, children }) => {
    return (
      <div>
        {foo}
        {bar}
        {children}
      </div>
    )
  }

  SpicyComponent.propTypes = {
    foo: PropTypes.number.isRequired,
    bar: PropTypes.string,
    children: PropTypes.node,
  }

  SpicyComponent.defaultProps = {
    bar: '',
    children: null,
  }

  export default SpicyComponent
  ```

- Avoid spread props as much as you can!

  > Why? 1) You’re more likely to pass unnecessary props down to components. 
  > 2) Unit tests become fragile

  Exceptions:

  - HOCs that proxy down props and hoist propTypes

  ```jsx
  const HOC = (WrappedComponent) => {
    return class Proxy extends React.Component {
      Proxy.propTypes = {
        text: PropTypes.string,
        isLoading: PropTypes.bool
      };

      render() {
        return <WrappedComponent {...this.props} />
      }
    }
  }
  ```
**[⬆ Back to top](#table-of-contents)**

## Refs

- Always use ref callbacks. eslint: [`react/no-string-refs`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/no-string-refs.md)

  ```jsx
  // bad
  <Foo
    ref="myRef"
  />

  // good
  <Foo
    ref={(ref) => { this.myRef = ref; }}
  />
  ```

## Parentheses

- Wrap JSX tags in parentheses when they span more than one line. eslint: [`react/jsx-wrap-multilines`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/jsx-wrap-multilines.md)

  ```jsx
  // bad
  render() {
    return <MyComponent variant="long body" foo="bar">
              <MyChild />
            </MyComponent>;
  }

  // good
  render() {
    return (
      <MyComponent variant="long body" foo="bar">
        <MyChild />
      </MyComponent>
    );
  }

  // good, when single line
  render() {
    const body = <div>hello</div>;
    return <MyComponent>{body}</MyComponent>;
  }
  ```

**[⬆ Back to top](#table-of-contents)**

## Tags

- Always self-close tags that have no children. eslint: [`react/self-closing-comp`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/self-closing-comp.md)

    ```jsx
    // bad
    <Foo variant="stuff"></Foo>

    // good
    <Foo variant="stuff" />
    ```

- If your component has multiline properties, close its tag on a new line. eslint: [`react/jsx-closing-bracket-location`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/jsx-closing-bracket-location.md)

  ```jsx
  // bad
  <Foo
    bar="bar"
    baz="baz" />

  // good
  <Foo
    bar="bar"
    baz="baz"
  />
  ```

**[⬆ Back to top](#table-of-contents)**

## Methods

- Use arrow functions to close over local variables. It is handy when you need to pass additional data to an event handler. Although, make sure they [do not massively hurt performance](https://www.bignerdranch.com/blog/choosing-the-best-approach-for-react-event-handlers/), in particular when passed to custom components that might be PureComponents, because they will trigger a possibly needless re-render every time.

  ```jsx
  function ItemList(props) {
    return (
      <ul>
        {props.items.map((item, index) => (
          <Item
            key={item.key}
            onClick={(event) => { doSomethingWith(event, item.name, index); }}
          />
        ))}
      </ul>
    );
  }
  ```

- Be sure to return a value in your `render` methods. eslint: [`react/require-render-return`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/require-render-return.md)

  ```jsx
  // bad
  render() {
    (<div />);
  }

  // good
  render() {
    return (<div />);
  }
  ```

- How to define `propTypes` and `defaultProps`

  ```jsx
  import React from 'react';
  import PropTypes from 'prop-types';

  const Link = ({id, url, text }) => {
    render() {
      return <a href={url} data-id={id}>{text}</a>;
    }
  }

  Link.propTypes = {
    id: PropTypes.number.isRequired,
    url: PropTypes.string.isRequired,
    text: PropTypes.string,
  };

  Link.defaultProps = {
    text: 'Hello World',
  };

  export default Link;
  ```
**[⬆ Back to top](#table-of-contents)**

## `isMounted`

- Do not use `isMounted`. eslint: [`react/no-is-mounted`](https://github.com/yannickcr/eslint-plugin-react/blob/master/docs/rules/no-is-mounted.md)

> Why? [`isMounted` is an anti-pattern][anti-pattern], is not available when
using ES6 classes, and is on its way to being officially deprecated.

[anti-pattern]: https://facebook.github.io/react/blog/2015/12/16/ismounted-antipattern.html

## CSS-in-JS

Our team uses 1 of 2 approaches to using CSS in React. No matter the method,
keep the following as the most important concerns:

  1. **CSS must be scoped.** CSS is inherently globally scoped. Thankfully it's
  scope is limited only to the CSS domain and not HTML or JavaScript.
  Some CSS is okay to be in the global scope, primarily: Utility classes. These
  are meant to be used by any component - no matter their purpose. You want to
  scope all of your other classes because you want to avoid styles bleeding over
  into other components/pages.
  2. **CSS must be portable.** Compose your CSS with the expectation that
  another developer will ask to use the same style you made. A reuseable button
  style is very valueable and requires very little extra work. You also want
  your style to continue to work on a component if a `<span>` is moved or
  removed.
  3. **CSS must be readable, findable, and maintainable.** Inline styles left
  all over a component may be the quickest way to achieve scoped and portable
  CSS, but it's _hell_ for another person to find, fix, and/or change. Have your
  CSS-in-JS live in the same area that is set by exisiting components. Look at
  other components and model after them. If you don't know which component to
  model from, _ask your team_. It'll come up in a future code review anyway -
  save yourself the embarassment 😉

### Approach 1: CSS Modules

CSS Modules is a great method to use in a React project - no matter the size of
the project.

This method has the following benefits:

- Achieves all three main concerns stated above.
- Separates your CSS converns from your JSX (HTML and JavaScript).
- Argueably the most portable method as all CSS is stored in a `.css/.scss` file.
that can be dropped in or directly imported on another component.
- Less of a learning-curve over `styled-components`.

Drawbacks:

- Relies heavily on your class naming conventions. You may start a project with
a naming convention in place that doesn't align with your module CSS.
- Tooling architecture may require you to debug situations where a 3rd party CSS.
library or JS library works with your module styling in strange ways.

### Approach 2: styled-components

This method has the following benefits:

- Achieves all three main concerns stated above but is more difficult to
maintian depending on the complexity of it.
- You can have your styles live closer to your JSX and remove the need to
maintain styles in completely different files.
- There may be situations where using `.css`/`.scss` isn't an option. CSS-in-JS
allows you to take control over styling in these cases.

Drawbacks:

- Giving CSS the power of JavaScript is not always a good thing. You'll need to
be concerned with the following:
  - [security](https://styled-components.com/docs/advanced#security)
pitfalls
    > Yep. So not only do you need to remember to sanitize all your inputs,
    **you need to make your designers do too**. And then trust them to keep
    doing it. Otherwise you’ll open up your site or app to a fun array of XSS
    attacks and possibly even arbitrary JavaScript execution.
    >
    > _Gufran Mirza - [Why Use CSS in JS, Benefits and Drawbacks](https://medium.com/@_imGufran/why-use-css-in-js-benefits-and-drawbacks-df40ab4ebef9)_
  - creating and maintaining unit tests
  - over-engineering
  - tracking changes/vulnerabilities in the to the [styled-components](https://github.com/styled-components/styled-components)
repo.
- Linting and syntax highlighting requires some work and will most likely need a
specific extension or library to get working.

# Media

## Icons

- SVG for icons whenever possible

## Tools

- Optimize SVGs with [SVGOMG](https://jakearchibald.github.io/svgomg/)
- [Kraken.io](https://kraken.io/web-interface) can be used for optimizing images but please leverage CDN services or Gulp tasks to automate whenever possible.

**[⬆ Back to top](#table-of-contents)**

# Typography

A good rule-of-thumb is to follow typography rules set by your design/brand team

## Fonts

Custom fonts should be loaded from the project itself and not through a CDN service.

> Why? If the CDN ever goes down or the file/license moves/expires, your font(s) will stop working

**[⬆ Back to top](#table-of-contents)**

# Performance

- Use [Lighthouse](https://web.dev/measure) (web app or browser extension) for perf testing. A minimum score of **70** for **Performance**, **Accessibility**, **Best Practices**, and **SEO** is expected.

- [Pingdom Speed Test](https://tools.pingdom.com/) or [Google PageSpeed](https://developers.google.com/speed) can be used to tst page speeds.

- We currently have to automated tools or dashboards for perf tests and site health.

# Accessibility

- Web pages are expected to meet [**"AA"** WCAG 2 requirements](https://www.w3.org/WAI/WCAG21/quickref/?currentsidebar=%23col_customize&levels=a%2Caaa).
- Follow the accessibility recommendations laid out in [this checklist](http://a11yproject.com/checklist.html).

## Tools

- [Lighthouse](https://web.dev/measure)
- [axe](https://chrome.google.com/webstore/detail/axe-web-accessibility-tes/lhdoppojpmngadmnindnejefpokejbdd)
- [WAVE](https://chrome.google.com/webstore/detail/wave-evaluation-tool/jbbplnpkjmmeebjpijfedlgcdilocofh)
- [Color Contrast Analyzer](https://chrome.google.com/webstore/detail/color-contrast-analyzer/dagdlcijhfbmgkjokkjicnnfimlebcll)

**[⬆ Back to top](#table-of-contents)**

# Tooling

## ESLint

**[⬆ Back to top](#table-of-contents)**

# Version control

## Git

All code is verioned with Git.

### Commits

- Commit early and often with good commit messages. Succinctly describe what
changes a commit introduces
- Do not use squash your commits
  > Why? We want to encourage commit messages that succinctly describe what
  > changes a commit introduces.
 
  > "... your commits paint a picture and tell a story. Squashing them loses
  > this. Sure, the changes are there, but you are not able to identify how a
  > change came to be."
  >  
  > _Holger Frohloff: [Best Practices on Doing Pull Requests](https://holgerfrohloff.de/best-practices-on-doing-pull-requests/)_

### Branching

Our branch naming conventions are set to have all branch names hyphenated `-` (no spaces or `_`), in lower-case and organised in folders by utilizing a `/` (only one allowed. `master` and `perf` expluded).

- `master`

  The `master` branch is where all branches spawn from. It contains the tested, polished, and most stable version of your project. Code in `master` directly mirrors what is in Production.

  The only branch that can be merged into `master` is `perf` and merging requires **approval**

  `master` can not be merged into any branch. Ever.

- `perf`

  This branch is used as the staging area for all other branches to be merged into before being promoted to `master`. It is treated as a mirror of `master` and is used for quality assurance, testing, stakeholder previews, and approvals.

- `wrike/`

  These branches come from issues submitted on Wrike and should include the Wrike ID # right after `issue/`. No description is needed as the Wrike # can be used to find the description.
  
  Example: `wrike/425591521` is the branch for [https://www.wrike.com/open.htm?id=425591521](https://www.wrike.com/open.htm?id=425591521)

- `feature/`

  A `feature` branch is a task which is neither captured in GitHub or Wrike but adds new fucntionality to a project. Just add a lower-case, hyphenated description that is not too long but still gives enough context for quick visual reference after `feature/`.

  Example: `feature/refactor-6-components-to-1`

- `release/`

  This is a branch that can be used as 1) a staging point for a number of other branches to be merged into it for a new, versioned, release of software 2) a historical state of the software. Following `release/` you add the version number of the release.

  Example: `release/1.2.14`

- `archive/`

  For projects that do not follow a semantic versioning process, there will be scenarios where you want to remove a full page, or pages, or piece(s) of functionality , but you want to keep a working state of the project in case you need to go back to reference that state. To do this, make a branch of `master` and name it `archive/` followed by a lower-case, hyphenated description that is not too long but still gives enough context for quick visual reference.

  Example: `archive/teal-and-green-brand-colours`

- `decommission/`

  These branches and `archive` branches work together. After making an `archive` branch from `master`, make a new branch off of `master` as the `decommission` branch and do all the work necessary to remove the functionality and/or pages from the project.

  Example: `decommission/teal-and-green-brand-colours`
  
  **Exceptions:** If the decommission work is captured in a Wrike task or GitHub Issue, follow the guidelines for a `wrike` branch or `issue` branch

- `issue/`

  These branches come from issues submitted on GitHub and should include the issue # right after `issue/`, followed by a lower-case, hyphenated description that is not too long but still gives enough context for quick visual reference. 
  
  Example: **Displaying errors in Radio/Checkbox groups #1393** would become `issue/1393-display-errors-radio-checkbox-groups`

- `fix/`
  
  A `fix` branch is a short-lived branch that addresses an issues like regression bugs, spelling mistakes, removing a `console.log()` that ended up in production code. After a `fix` branch has been merged into `master`, it can be safely removed.

  Example: `fix/product-card-typos`

**[⬆ Back to top](#table-of-contents)**

### Merging

- Never merge `master` into another branch
- Only `perf` can be merged into master. **_Requires code review and approval._**
- Merging a working branch into `perf` must be done through a
[GitHub Pull Request](#pull-requests--pr-). **_Requires code review and approval._**
- If your working branch becomes "stale" (has not had any commits in the
previous 3 weeks or longer), it is a _GREAT_ idea to check it out, and then
merge `perf` into it to see what conflicts may arise.
  > Why? Getting started on these conflicts early will save you, potentially, an
  > enormous amount of time from discovering the conflict when you complete your
  > work and do your Pull Request into `perf`.

**[⬆ Back to top](#table-of-contents)**

## GitHub

All source code is stored in [GitHub](https://github.com/)

### Pull Requests "PR"

- Require 1 minimum of 1 developer team member to [review code](#code-reviews).
- Require code review approval to merge.
- Do not use **Squash and Merge**.
  > Why? We encourage commit messages that succinctly describe what changes a
  > commit introduces.
- We use before-commit hooks in Git to test your branch before it gets merged.
- If you're creating a PR for a Wrike task, please add the Wrike's link in the
description of the PR.
- If the PR has a template, please follow the instructions in the template. If
the template does not accurately cover what needs to be covered, please flag it
with your team.
- The person merging the PR shouldn’t be the one who opened it.

### Code reviews

#### Reviewer

- Remember the following when adding comments on a code review:
  - Don't make the review personal. Be respectful and remember that context is easily lost.
    - you can always talk face-to-face with someone first or review their code
    sitting together (physically or virtually) so that context is not lost.
  - It's helpful to add the reasoning for the change you are requesting.
  - If you do not understand an approach someone has taken, ask for their
  reasoning - this may be an opportunity for you to learn something as well.

#### Reviewee

> "Remember: [You are not your code]."
>  
> _Holger Frohloff [How do you review a pull request?](https://holgerfrohloff.de/how-do-you-review-a-pull-request/)_

- Try not to take code review comments as personal attacks (unless there are
litterally perosnal attacks in the code review comments - that's something that
your leader should definitely be made aware of). Try to think of code reviews as
two artists getting together to create something even better; if Mozart and Post
Malone were to work together on the same song - imagine the incredible end
result!

**[⬆ Back to top](#table-of-contents)**

# Localization

Our projects are served in `en-CA` and `fr-CA`.

# Deployment/Integration

Infrastructure is beyond the scope of this document.

# Documentation

## In-line code comments

- Code is written and maintained by people. Ensure your code is descriptive,
  well commented, and approachable by others. Great code comments convey context
  or purpose. Do not simply reiterate a component or class name.

  Be sure to write in complete sentences for larger comments and succinct
  phrases for general notes.

- Code comments should not appear in production code that is served to the
  client. Ensure that your build process is leaving in comments in developed
  code, but outputting production code with comments stripped out.
  `console.log()` debugging messages should also never appear on production code
  _except under special, urgent circumstances_.

## README documentation

Documentation is kept in README.md (please name these files `README.md`) files
in projects and should bbe kept fresh and accurate.

# Kudos

This document has been largely based off of the fantastic work by
[Brad Frost](https://github.com/bradfrost/):
  [https://github.com/bradfrost/frontend-guidelines-questionnaire](https://github.com/bradfrost/frontend-guidelines-questionnaire)

  **[⬆ Back to top](#table-of-contents)**
