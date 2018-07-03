# Question 1
Areas addressed: JAVASCRIPT, DOM MANIPULATION

## Image Gallery
An image gallery is a set of images with corresponding _remove_ buttons. This is the HTML code for a gallery with two images:

```
<div class="image">
  <img src="https://goo.gl/kjzfbE" alt="First">
  <button class="remove">X</button>
</div>
<div class="image">
  <img src="https://goo.gl/d2JncW" alt="Second">
  <button class="remove">X</button>
</div>
```

Implement the _setup_ function that registers a click event handler and implements the following logic: When the button of class _remove_ is clicked, its parent _DIV_ element should be removed from the gallery.

For example, after the first image has been removed from the gallery above, it's HTML code should look like this:

```
<div class="image">
  <img src="https://goo.gl/d2JncW" alt="Second">
  <button class="remove">X</button>
</div>
```

You may NOT use any external libraries for the completion of this question.