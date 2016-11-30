---
title: About
date: 2000-01-01 12:00:00
---

These Base Styles are meant as a baseline for our frontend.

### Goals

- Unify fonts, colors and common elements
- Unopinionated and flexible
- 0 kb dependency - _only expose mixins_ and allows gradual rollout

Feel free to extend and override it. It's not an UI framework, _but it could serve as a base for one)_. _Pattern library_ should take care of cataloging use of this in the wild.

### Getting started

Install with npm:

```bash
npm i apiary-base-styles -S
```

Import into your Stylus file:

```stylus
@import 'apiary-base-styles'
```

Now you can start using parts of Base Styles - all of them are prefixed with `$`, see reference below.
