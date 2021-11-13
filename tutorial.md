---
title: Tutorial
layout: page
toc: true
---
# Tutorial
## Getting Started

### Setting the Theme

To start with Inkwell, put it in your website as a `remote_theme` in `_config.yml`:

```yaml
remote_theme: ManchesterMachineMakers/inkwell
```

### Setting Configuration

Set the following properties in `_config.yml` so that everything functions properly:

```yaml
title: Your Site Title
baseurl: /path/to/your/site
icon: /path/to/icon.svg
```

_(Note: the icon does not need to be SVG.)_

### Adding a Landing Page

You will want to convert your main page (`index.md` or the like) into a landing page, which has a jumbotron. To do this, add a whole whack of frontmatter, following this template:

```yaml
layout: landing
title: Page Title
header:
    title: "Your Site's Title"
    slogan: Your slogan here
    logo: /path/to/logo
    buttons:
        - title: Button Title
          url: '/path/to/page'
        - title: Other Button
          url: '/path/to/page'
```

If you want a table of contents sidebar, add `toc: true` as well.

### Creating the Navbar

To add links to the navbar, create `_data/navigation.yml` with a list of links, like so:

```yaml
- name: Home
  path: /
- name: Other Page
  path: /other-page
```

### Setting Page Layouts

All non-landing pages should use the `page` layout, like so:

```yaml
layout: page
toc: true # Or false, if you don't want one
```

The `default` layout is not meant to be used directly.

## Customization

To customize the styling, create `assets/css/main.scss`, `_sass/main.scss`, and `_sass/variables.css`.

`assets/css/main.scss`:

```scss
---
---
@import "main";
```

`_sass/main.scss`:

```scss
@import "inkwell/variables";
@import "variables";
@import "inkwell/flex";
@import "inkwell/syntax-highlighting";
@import "inkwell/nav";
@import "inkwell/base";
```

And in `_sass/variables.scss`, customize the variables, as below:

```scss
$primary: #0090f7; // Primary color
$primary-alt: #006bf7; // Alternate primary color (generally should be darker)
$primary-fg: #ffffff; // Foreground color for elements using the primary color as their background (there's probably a more succinct way of wording that)
$gradient: linear-gradient(91.71deg, $primary-alt 0%, $primary 100%); // Gradient to use for everything
$responsive-breakpoint: 768px; // Responsive breakpoint width
```

