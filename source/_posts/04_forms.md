---
title: Forms
date: 3005-01-01 12:00:00
---

Basic styling for forms is available under `$apiaryForm()` mixin

```stylus
.apiaryForm
  $apiaryForm()
```

<div class="row">
  <div class="col-xs-12 col-md-6">
    <form class="apiaryForm">
      <label for="fullName">Full Name</label>
      <input type="text" name="fullName" id="fullName" value="John Doe">
      <label for="email2">Email Address</label>
      <input type="email" name="email" id="email2" value="invalid email@" required>
      <label for="phoneNumber">Phone Number</label>
      <input type="tel" name="phoneNumber" id="phoneNumber" placeholder="555-1234">
      <input type="submit" value="Contact Me">
    </form>
  </div>
  <div class="col-xs-12 col-md-6">
    ```html
    <form class="apiaryForm">
      <label for="fullName">Full Name</label>
      <input type="text" name="fullName" id="fullName" value="John Doe">
      <label for="email">Email Address</label>
      <input type="email" name="email" id="email2" value="invalid email@" required>
      <label for="phoneNumber">Phone Number</label>
      <input type="tel" name="phoneNumber" id="phoneNumber" placeholder="555-1234">
      <input type="submit" value="Contact Me">
    </form>
    ```
  </div>
</div>

<hr />

<div class="row">
  <div class="col-xs-12 col-md-6">
    <form class="apiaryForm">
      <fieldset>
        <legend>A compact inline form</legend>
        <label for="email">Email</label>
        <input type="email" name="email" id="email" placeholder="john@example.com">
        <label for="password">Password</label>
        <input type="password" name="password" id="password" placeholder="password">
        <label for="remember">
          <input id="remember" type="checkbox"> Remember me
        </label>
        <button type="submit">Sign in</button>
      </fieldset>
    </form>
  </div>
  <div class="col-xs-12 col-md-6">
    ```html
    <form class="apiaryForm">
      <fieldset>
        <legend>A compact inline form</legend>
        <label for="email">Email</label>
        <input type="email" name="email" id="email" placeholder="john@example.com">
        <label for="password">Password</label>
        <input type="password" name="password" id="password" placeholder="password">
        <label for="remember">
          <input id="remember" type="checkbox"> Remember me
        </label>
        <button type="submit">Sign in</button>
      </fieldset>
    </form>
    ```
  </div>
</div>
