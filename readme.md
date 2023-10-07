# 🥾 BootsLace

This is an hybrid between [Bootstrap](https://getbootstrap.com) (CSS framework) and [Shoelace](https://shoelace.style/) (Web Components library).

## Problem supposed to solve

I make websites by using [Publii CMS](https://getpublii.com), which is a great solution for managing websites and content on your PC, it generates fast static websites, and has a bunch of usefull features, but it lacks easy ways to create more "advanced" layouts (like a two/three column layout 😁 ). Useless to say that one can use it however you want!

So I want a CSS framework, but I'd like it to be lightweight and to easily pick single components I need, without importing all the JS library.

> Note: this is a work in progress, I'll test it and compare loading times + Core Web Vitals with the full version of Bootstrap 5 and post the results.

## Usage

Download the `dist` folder and add the following code to the header of your html file (adjust the paths as needed):

```html
<link rel="stylesheet" href="path/to/dist/css/bootslace-light.min.css" />

<style>
  :not(:defined) {
    visibility: hidden;
  }
</style>

<script type="module" data-shoelace="path/to/dist/shoelace">
  /* import the components you need, e.g.: */
  import "path/to/dist/shoelace/components/button/button.js";
  import "path/to/dist/dist/shoelace/components/card/card.js";
  import "path/to/dist/dist/shoelace/components/details/details.js";
</script>
```

For more info about components check the [shoelace documentation](https://shoelace.style/components/button).
