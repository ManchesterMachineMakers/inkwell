---
layout: landing
header:
    title: Inkwell
    slogan: A modern theme for Jekyll sites
    logo: /assets/InkwellLogo.svg
    buttons:
        - title: Get Started
          url: '/tutorial'
        - title: Components
          url: '/components'
        - title: GitHub
          url: 'https://github.com/aleksrutins/inkwell'
title: "Home"
toc: true
---

# Inkwell
Inkwell is a modern theme for Jekyll sites.

## Features

### Landing Page

Inkwell's `landing` layout allows you to have a nicely-formatted landing page with a jumbotron and navigation buttons (like this page).

### Table of Contents
Any page with a layout other than `default` and with `toc: true` in its Frontmatter will get an automatically-generated responsive table-of-contents sidebar.

### Responsive
All elements should be responsive.
If you see anything not on the following list that isn't responsive, please [open an issue](https://github.com/aleksrutins/inkwell/issues).
#### Items To Be Implemented
- Sidebar

### Modern Code Styling
```js
function doSomething(argument) {
  const el = document.createElement("div");
  el.appendChild(document.createTextNode(argument));
  document.body.appendChild(el);
}
```
See more examples here:

<a class="btn btn-go" href="{{'/components#syntax-highlighting' | relative_url}}">Components: Syntax Highlighting</a>