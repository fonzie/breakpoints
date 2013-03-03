# Breakpoints

Media queries for working with different devices. The breakpoints for each query can
be customized so that they match your grid.

## Installation

```
fonzie install breakpoints
```

Then import them:

```
@import "breakpoints";
```

## Usage

The mixins make use of content blocks in mixins. Just pick a mixin and use it anywhere.

```scss
@include mobile {
  body {
    background: #eee;
    padding: 40px;
  }
}

.box {
  width: 500px;
  @include tablet-portrait {
    width: 250px;
  }
  @include mobile {
    width: 100px;
  }
}
```

You can adjust the points used for these media queries by changing variables:

```scss
$mq-mobile-portrait: 340px;
$mq-mobile-landscape: 500px;
$mq-tablet-portrait: 700px;
$mq-tablet-landscape: 900px;
$mq-desktop: 1100px;
```

## Mixins

There are a number of mixins available for targeting above, below and on a breakpoint.

  * mobile
  * mobile-portrait
  * mobile-portrait-and-below
  * mobile-portrait-and-up
  * mobile-landscape
  * mobile-landscape-and-below
  * mobile-landscape-and-up
  * tablet
  * tablet-portrait 
  * tablet-portrait-and-below
  * tablet-portrait-and-up
  * tablet-landscape
  * tablet-landscape-and-below 
  * tablet-landscape-and-up
  * desktop-and-up 
  * desktop-and-below
  * desktop