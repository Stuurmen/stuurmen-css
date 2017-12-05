Stuurmen CSS
==================================

Front-end boilerplate for projects by [Stuurmen][stuur.men].

## Requirements

| Prerequisite    | How to check  | How to install                   |
| --------------- | ------------- | -------------------------------- |
| Node.js 4.1.1   | `node -v`     | [nodejs.org](https://nodejs.org) |

## Getting started

1.  **Get the latest node modules**
    1.  `npm install -g npm-check-updates`
    2.  `npm-check-updates -u`
    3.  `npm install`

2a.  **Test linting and building**
    -   `npm run test`
2b.  **Lint SCSS**
    -   `npm run lint`
2c.  **Build main.css**
    -   `npm run scss**

## CSS

-   We use [Sass](http://sass-lang.com) for our CSS Preprocessor
-   [itcss](http://itcss.io) CSS architecture
-   [BEMIT](http://www.jamesturneronline.net/blog/bemit-naming-convention.html) naming convention
-   [More Transparent UI Code with Namespaces](http://csswizardry.com/2015/03/more-transparent-ui-code-with-namespaces)
-   [Sass MQ](https://github.com/sass-mq/sass-mq) for media queries

### Sass import order

*   **Settings:** Global variables, site-wide settings, config switches, etc.
*   **Tools:** Site-wide mixins and functions.
*   **Generic:** Low-specificity, far-reaching rulesets (e.g. resets).
*   **Elements:** Unclassed HTML elements (e.g. `a {}`, `blockquote {}`, `address {}`).
*   **Objects:** Objects, abstractions, and design patterns (e.g. `.o-media {}`).
*   **Components:** Discrete, complete chunks of UI (e.g. `.c-carousel {}`).
*   **Utilities:** High-specificity, very explicit selectors. Overrides and helper
  classes (e.g. `.u-hidden {}`).
*   **Templates Custom templating

### Grid

We are using a simple flexbox grid.

**Usage**

Insert a `o-layout` block and add `o-layout__item` elements inside it. Build colums by using e.g. u-1, u-6 etc.

-   Include the grid mixins in your components classes.
-   Create custom width grid items by including the `layout__item` mixin and adding the widths you need or just include the helpers mixins with fractions like names.
-   Add media queries, on the helpers mixins or on your custom components to change the grid items widths, for your content, on different screen sizes.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/deJong/stuurmen-css).

## Authors

* **Stijn de Jong** - *Initial work* - [Stuurmen](https://github.com/deJong)
