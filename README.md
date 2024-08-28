# CSS Reset

This is a customized version of [Josh W. Comeau's Modern CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/) that I have adapted for my projects. This reset ensures a consistent baseline across browsers, while adding a few tweaks to enhance the user experience and maintain clean design defaults.

## CSS Reset Code

```css
/* 1. Use a more intuitive box-sizing model */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* 2. Remove default margin and standardize line height */
* {
  margin: 0;
  line-height: calc(1em + 0.5rem);
}

/* 3. Improve text rendering for smoother fonts */
body {
  -webkit-font-smoothing: antialiased;
}

/* 4. Improve media defaults for fluid responsiveness */
img,
picture,
video,
canvas,
svg {
  display: block;
  max-width: 100%;
}

/* 5. Inherit font settings for form elements */
input,
button,
textarea,
select {
  font: inherit;
}

/* 6. Prevent text overflow and handle hyphenation */
p,
h1,
h2,
h3,
h4,
h5,
h6 {
  overflow-wrap: break-word;
  hyphens: auto;
}
```

## Key Modifications:

- **Enhanced Line Height:** The line-height is calculated dynamically using `calc(1em + 0.5rem)`, offering better vertical rhythm across different font sizes.
- **Hyphenation and Overflow Prevention:** Added `hyphens: auto` and `overflow-wrap: break-word` to prevent text overflow and improve readability for long words.
- **Inherited Font in Forms:** Ensures form elements inherit the font from their surroundings for consistent typography across the page.

## No-Comment Version for Easy Pasting

```css
*,
*::before,
*::after {
  box-sizing: border-box;
}

* {
  margin: 0;
  line-height: calc(1em + 0.5rem);
}

body {
  -webkit-font-smoothing: antialiased;
}

img,
picture,
video,
canvas,
svg {
  display: block;
  max-width: 100%;
}

input,
button,
textarea,
select {
  font: inherit;
}

p,
h1,
h2,
h3,
h4,
h5,
h6 {
  overflow-wrap: break-word;
  hyphens: auto;
}
```

## The Original Reset

This reset is based on the following core principles from Josh W. Comeau's original reset:

```css
/*
  1. Use a more-intuitive box-sizing model.
*/
*,
*::before,
*::after {
  box-sizing: border-box;
}
/*
  2. Remove default margin
*/
* {
  margin: 0;
}
/*
  Typographic tweaks!
  3. Add accessible line-height
  4. Improve text rendering
*/
body {
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
}
/*
  5. Improve media defaults
*/
img,
picture,
video,
canvas,
svg {
  display: block;
  max-width: 100%;
}
/*
  6. Remove built-in form typography styles
*/
input,
button,
textarea,
select {
  font: inherit;
}
/*
  7. Avoid text overflows
*/
p,
h1,
h2,
h3,
h4,
h5,
h6 {
  overflow-wrap: break-word;
}
/*
  8. Create a root stacking context
*/
#root,
#__next {
  isolation: isolate;
}
```
