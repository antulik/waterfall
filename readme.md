# jQuery.waterfall + modification by antulik

- It provides functionality for column based layout.
- It's [Pinterest](http://pinterest.com)-like layout with fluid width of columns. 
- Fast, tiny, reliable and free alternative to [isotope masonry column shift](http://isotope.metafizzy.co/custom-layout-modes/masonry-column-shift.html) layout.
- This is a fork of [dfcreative/waterfall](https://github.com/dfcreative/waterfall) version.  In this version you can easily build custom responsive layouts and replace CSS media queries.

## Getting started

**Requires** [jQuery](http://jquery.com/) or [Zepro.js](http://zeptojs.com/)

(Optional) Global default configuration.

```
// add this before library is loaded
window.waterfall = {
  // ...
};
```

Add waterfall script to your page

```html
<script src="/jquery.waterfall.js"></script>
```

Now you can start using it:

```html
<div class='waterfall'>
    <div>One</div>
    <div>Two</div>
    <div>Three</div>
</div>
```

## Customise layout
with html data-* attributes

### container

- **data-max-cols** - maximum number of columns allowed (default=null)
- **data-col-min-width** - minimum width of each column (default=300)

### element

- **data-span** - number of columns to span the element (default=1)
	- allowed values: all or any Number
- **data-column**  - specific column to place the element in (default=any)
	- allowed values: any,left,right,first,last or any Number

## Advanced usage & Responsive layout

**data-span** and **data-column** can have multiple values separated by `,`(comma): 

- `data-span='1,all'` - **span=all** when number of columns is 2, otherwise **span=1**
- `data-column='right,any,any'` - **column=any** when number of columns is 2 or 3, otherwise **column=right**

**Syntax** 

`data-span|data-column=default,2 columns,3 columns,4 columns, ...`

For example when the current number of columns in the layout is 2, then value from `2 columns` will be used. If it is missing or blank then default value will be used.





