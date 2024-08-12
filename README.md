# CSS Reset

A slightly tweaked version of Josh W Comeu's [Modern CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/) that I've been using.

``` css
*, ::before, ::after {
	box-sizing: border-box;
}

* {
	margin: 0;
	line-height: calc(1em + 0.5rem);
}

body {
  -webkit-font-smoothing: antialiased;
}

img, picture, video, canvas, svg {
  display: block;
  max-width: 100%;
}

input, button, textarea, select {
  font: inherit;
}

p, h1, h2, h3, h4, h5, h6{
  overflow-wrap: break-word;
  hyphens: auto;
}
```
