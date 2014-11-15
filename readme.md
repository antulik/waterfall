# jQuery.waterfall + modification by antulik

This is a fork of [dfcreative/waterfall](https://github.com/dfcreative/waterfall) version.


jQuery.waterfall is [Pinterest](http://pinterest.com)-like layout with fluid width of columns. Fast, tiny, reliable and free alternative to [isotope masonry column shift](http://isotope.metafizzy.co/custom-layout-modes/masonry-column-shift.html) layout.

## Usage

### Setup

**Requires** [jQuery](http://jquery.com/) or [Zepro.js](http://zeptojs.com/)

Global default configuration.

```
// add this before library is loaded
window.waterfall = {
  // ...
};
```

Add script to your page

```
<script src="/jquery.waterfall.js"></script>
```

Now you can start using it:

```
<div class='waterfall'>
    <div>One</div>
    <div>Two</div>
    <div>Three</div>
</div>
```
