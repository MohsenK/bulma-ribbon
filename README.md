# bulma-ribbon
Bulma's extension to show a ribbon on boxes
(find all my bulma's extensions [here](https://github.com/Wikiki/bulma-extensions))

![Ribbon Element](https://img4.hostingpics.net/pics/737717ScreenShot20170810at095724.png)

Usage
---
```html
<div class="columns is-multiline">
  <div class="column">
    <div class="box has-ribbon">
      <div class="ribbon">Default</div>
      Box content
    </div>
  </div>
  <div class="column">

    <div class="box has-ribbon">
      <div class="ribbon is-primary">Primary</div>
      Box content
    </div>
  </div>
  <div class="column">
    <div class="box has-ribbon">
      <div class="ribbon is-warning">Warning</div>
      Box content
    </div>
  </div>
  <div class="column">
    <div class="box has-ribbon">
      <div class="ribbon is-danger">Danger</div>
      Box content
    </div>
  </div>
</div>
<div class="columns is-multiline">
  <div class="column">
  <div class="box has-ribbon is-small">
    <div class="ribbon is-small is-primary">Small ribbon</div>
    Box content
  </div>
</div>

  <div class="column">
    <div class="box has-ribbon is-small">
      <div class="ribbon is-medium is-primary">Medium ribbon</div>
      Box content
    </div>
  </div>

  <div class="column">
    <div class="box has-ribbon is-small">
      <div class="ribbon is-large is-primary">Large ribbon</div>
      Box content
    </div>
  </div>
</div>
<div class="columns is-multiline">
  <div class="column">
    <div class="box has-ribbon-left is-small">
      <div class="ribbon is-small is-primary">Left ribbon</div>
      Box content
    </div>
  </div>

  <div class="column">
    <div class="box has-ribbon-bottom is-small">
      <div class="ribbon is-small is-primary">Bottom ribbon</div>
      Box content
    </div>
  </div>
</div>
```

Modifiers
---
You can use standards color modifiers and you can change the ribbon's position using the following modifiers in replacement of has-ribbon class:
- has-ribbon-left
- has-ribbon-bottom

Variables
---
This extension uses the following variables

Name | Description | Default value    
-----|-------------|---------------
$ribbon-color | Default ribbon text color | $grey-darker
$ribbon-background-color | Default background color of the ribbon | $white
$ribbon-border-color | Ribbon default border color | $grey-lighter

Demo
---
You can find a demo [here](https://codepen.io/wikiki/pen/XagrqJ)

Integration
---
- Clone the [bulma repo](https://github.com/jgthms/bulma)
- Under the `sass` folder, create a new folder called `extensions`
- In this new folder, create a new file `ribbon.sass`
- Copy the code form the `bulma-ribbon repo`'s [ribbon.sass](https://github.com/Wikiki/bulma-ribbon/blob/master/ribbon.sass) file into your new file
- In the same folder create a new file `_all.sass` (this is not required, but will help when you add more extensions)
- In this file add this code:
```
@charset "utf-8"

@import "ribbon.sass"
```
At the end of the `bulma.sass` file, add this line: `@import "sass/extensions/_all"`

Now, you can just build the bulma project with `npm run build`, and the output will be available in the `css folder`.
