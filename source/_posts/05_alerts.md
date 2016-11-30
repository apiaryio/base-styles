---
title: Alert boxes
date: 4005-01-01 12:00:00
---

Alert boxes are important part of the UI.

```stylus
.alert
  $alert()
```

This will add some basic styling to `.alert` and adds BEM modifiers `__success`, `__warning`, `__error` and `__info`.

<div class="alert alert__success">Success message</div>
<div class="alert alert__warning">Warning message</div>
<div class="alert alert__error">Error message</div>
<div class="alert alert__info">Info message</div>

```html
<div class="alert alert__success">Success message</div>
<div class="alert alert__warning">Warning message</div>
<div class="alert alert__error">Error message</div>
<div class="alert alert__info">Info message</div>
```

Alert headings and icon/body are also available. Use `--figure` and `--body` as a [media object](http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/):

<div class="alert alert__success">
  <div class="alert--figure">
    <!-- Any icon/image is allowed here -->
    <i class="icono-checkCircle"></i>
  </div>
  <div class="alert--body">
    <div class="alert--heading">Heading</div>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin imperdiet ex a quam commodo semper. Sed ac nulla in velit feugiat malesuada. Donec vel volutpat arcu, vitae ullamcorper sem. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
  </div>
</div>

```html
<div class="alert alert__success">
  <div class="alert--figure">
    <!-- Any icon/image is allowed here -->
    <i class="icono-checkCircle"></i>
  </div>
  <div class="alert--body">
    <div class="alert--heading">Heading</div>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin imperdiet ex a quam commodo semper. Sed ac nulla in velit feugiat malesuada. Donec vel volutpat arcu, vitae ullamcorper sem. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
  </div>
</div>
```

<div class="alert alert__info">
  <div class="alert--heading">Heading</div>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin imperdiet ex a quam commodo semper. Sed ac nulla in velit feugiat malesuada. Donec vel volutpat arcu, vitae ullamcorper sem. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
</div>

```html
<div class="alert alert__info">
  <div class="alert--heading">Heading</div>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin imperdiet ex a quam commodo semper. Sed ac nulla in velit feugiat malesuada. Donec vel volutpat arcu, vitae ullamcorper sem. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
</div>
```

Don't forget to use `<p>` for content when using `--heading`.
