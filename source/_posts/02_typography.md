---
title: Typography
date: 2002-01-01 12:00:00
---

You can setup basic styles for text like color, line-height and font-weight by calling `$apiaryBase` mixin like so:

```stylus
$apiaryBase()
```

It will setup

- default font size
- set box-sizing to border-box
- padding, margin 0 on html/body
- link colors
- responsive image resizing

Easiest way to get these fonts into your website is embedding them directly from Google Fonts:

```html
<link href="https://fonts.googleapis.com/css?family=Source+Code+Pro|Source+Sans+Pro:200,400,600" rel="stylesheet">
```

For production, [better ways are recommended](https://www.zachleat.com/web/comprehensive-webfonts/).

<div class="typoBox typoBox--sans">
  <h3>Source Sans</h3>
  <p>General use font</p>
  ```stylus
  p
    font-family $baseFont
  ```
  <div class="row between-xs">
    <div class="typoBox__content typoBox__content--sans typoBox__content--100 col-xs-12 col-md-4">abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890</div>
    <div class="typoBox__content typoBox__content--sans typoBox__content--400 col-xs-12 col-md-4">abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890</div>
    <div class="typoBox__content typoBox__content--sans typoBox__content--600 col-xs-12 col-md-4">abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890</div>
  </div>
</div>

<hr />

<div class="typoBox typoBox--mono">
  <h3>Source Code Pro</h3>
  <p>For code examples or editor</p>
  ```stylus
  code
    font-family $monoFont
  ```
  <div class="typoBox__content typoBox__content--mono typoBox__content--400">abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890?!.-</div>
</div>

<hr />

## Heading styles
Few predefined heading styles

<div class="typoPreview">
  <h1><code>h1</code>Fast-track your API Design</h1>
  <h2><code>h2</code>Fast-track your API Design</h2>
  <h3><code>h3</code>Fast-track your API Design</h3>
  <h4><code>h4</code>Fast-track your API Design</h4>
  <h5><code>h5</code>Fast-track your API Design</h5>
  <h6><code>h6</code>Fast-track your API Design</h6>
</div>

```stylus
$apiaryHeadings() /* To setup h1 to h6 styles */
```
