---
title: Buttons
date: 2003-01-01 12:00:00
---

Style Guide comes with few predefined button styles and an unified button baseline mixin:

```html
<button class="button--primary"><div>Hello world</div></button>
```
<button class="button--primary"><div>Hello world</div></button>
<button class="button--secondary"><div>Hello world</div></button>
<button class="button--link"><div>Hello world</div></button>
<button class="button--primary" disabled><div>Disabled button</div></button>


```html
<a href="javascript:;" class="button--primary" role="button">Hello world</a>
```
<a href="javascript:;" class="button--primary" role="button">Hello world</a>
<a href="javascript:;" class="button--secondary" role="button">Hello world</a>
<a href="javascript:;" class="button--link" role="button">Hello world</a>
<a href="javascript:;" class="button--primary" role="button" disabled>Disabled doesn't work for anchor tags</a>

```html
<input type="button" class="button--primary" value="Hello world" />
```
<input type="button" class="button--primary" value="Hello world" />
<input type="button" class="button--secondary" value="Hello world" />
<input type="button" class="button--link" value="Hello world" />
<input type="button" class="button--primary" value="Disabled button" disabled />

**PROTIP**: [Use `<button>` element for UI](https://www.youtube.com/watch?v=CZGqnp06DnI)

```stylus
// 4 predefined button styles
.button--primary
  $apiaryButtonPrimary()
.button--secondary
  $apiaryButtonSecondary()
.button--link
  $apiaryButtonLink() // Link only button
```

### New button styles

You can easily create new combination if needed with `$apiaryButton()` mixin with single argument `fontSize` (defaults to `13px`)

```stylus
.button--custom
  $apiaryButton(fontSize: 18px)
  background-color #264653
  &:hover
    background-color #2A9D8F
```
<button class="button--custom"><div>New button style!</div></button>

There are 3 supported HTML markups:
```html
<!-- use for links -->
<a href="#" class="button--primary">Hello world</a>
<!-- use for actions in UI -->
<button class="button--secondary"><div>Hello world</div></button>
<!-- use in forms -->
<input type="button" class="button--secondary" value="Hello world" />
```

### Loading indicator element
Use `$loadingIndicator()` mixin with `color` and `size` options:


```stylus
.loadingIndicator
  $loadingIndicator()
  &--big
    $loadingIndicator(size: 12px)
  &--blue
    $loadingIndicator(color: $primaryColor)
```

```html
<div class="loadingIndicator"></div>
<div class="loadingIndicator loadingIndicator--big"></div>
<div class="loadingIndicator loadingIndicator--blue"></div>
```

Default
<div class="loadingIndicator"></div>

With specified `size`
<div class="loadingIndicator loadingIndicator--big"></div>

With specified `color`
<div class="loadingIndicator loadingIndicator--blue"></div>
