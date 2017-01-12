---
title: Alert boxes
date: 4005-01-01 12:00:00
---

Alert boxes are important part of the UI.

```stylus
.alert
  $alert()
```

This will add some basic styling to `.alert` and adds BEM modifiers `--success`, `--warning`, `--error` and `--info`.

<div class="alert alert--success">Success message</div>
<div class="alert alert--warning">Warning message</div>
<div class="alert alert--error">Error message</div>
<div class="alert alert--info">Info message</div>

```html
<div class="alert alert--success">Success message</div>
<div class="alert alert--warning">Warning message</div>
<div class="alert alert--error">Error message</div>
<div class="alert alert--info">Info message</div>
```

Alert headings and icon/body are also available. Use `__figure` and `__body` as a [media object](http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/):

<div class="alert alert--success">
  <div class="alert__figure">
    <!-- Any icon/image is allowed here -->
    <i class="icono-checkCircle"></i>
  </div>
  <div class="alert__body">
    <div class="alert__heading">Heading</div>
    <p>Lorem ipsum <a href="javascript:;">dolor sit amet</a>, consectetur adipiscing elit. Proin imperdiet ex a quam commodo semper. Sed ac nulla in velit feugiat malesuada. Donec vel volutpat arcu, vitae ullamcorper sem. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
  </div>
</div>

```html
<div class="alert alert--success">
  <div class="alert__figure">
    <!-- Any icon/image is allowed here -->
    <i class="icono-checkCircle"></i>
  </div>
  <div class="alert__body">
    <div class="alert__heading">Heading</div>
    <p>Lorem ipsum <a href="javascript:;">dolor sit amet</a>, consectetur adipiscing elit. Proin imperdiet ex a quam commodo semper. Sed ac nulla in velit feugiat malesuada. Donec vel volutpat arcu, vitae ullamcorper sem. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
  </div>
</div>
```

<div class="alert alert--info">
  <div class="alert__heading">Heading</div>
  <p>Lorem ipsum dolor sit amet, <a href="javascript:;">dolor sit amet</a>. Proin imperdiet ex a quam commodo semper. Sed ac nulla in velit feugiat malesuada. Donec vel volutpat arcu, vitae ullamcorper sem. Lorem ipsum dolor sit amet, <a href="javascript:;">dolor sit amet</a>.</p>
</div>

```html
<div class="alert alert--info">
  <div class="alert__heading">Heading</div>
  <p>Lorem ipsum dolor sit amet, <a href="javascript:;">dolor sit amet</a>. Proin imperdiet ex a quam commodo semper. Sed ac nulla in velit feugiat malesuada. Donec vel volutpat arcu, vitae ullamcorper sem. Lorem ipsum dolor sit amet, <a href="javascript:;">dolor sit amet</a>.</p>
</div>
```

Don't forget to use `<p>` for content when using `__heading`.
