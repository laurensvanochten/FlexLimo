# FlexLimo
Simple CSS grid based of Lemonade.im with support for Flexbox

The entire grid is based on Lemonade.im which can be found:

GIT: https://github.com/dope/lemonade
WWW: http://lemonade.im

---

FlexLimo is based on Lemonade.im and extends the original grid with flexbox support. 

FlexLimo works the same as Lemonade.im with a few extra additions.

Blog post with some background info can be found [here](http://tutorial.thekitchn.eu/flexlimo/)

## Include it
In order to use it include it in you html

`<link rel="stylesheet" type="text/css" href="css/flexlimo.css">`

## Add it
Add the classes to your HTML. Where the original version of Lemonade uses `.frame`, FlexLimo uses `.flexbox` for the wrapper div. 

In order to set the width of your elements you will still be using `.bit-` classes as introduced by the original verison of Lemonade (bit-1 equals 100%, bit-2 equals 50% etc).

In order to set the order of your elements you need to add `.flex-` classes to your elements (flex-1 means order 1, flex-2 means order 2 etc).

```html
 <div class="container flexbox">
            <div class="bit-3 flex-2 flex-1-sm box">box 1 - aligned top</div>
            <div class="bit-3 flex-3 flex-2-sm box">box 2 - aligned center</div>
            <div class="bit-3 flex-1 flex-3-sm box">box 3 - aligned bottom</div>
</div>
```

## More options

In order to control the order of content on various screen sizes you can add the following classes to your html elements:

```css
.flex(nth)-sm /* below 480px */
.flex(nth)-med  /* 480px till 800px */
.flex(nth)-lrg  /* 800px till 1100px */
```

You will need to replace (nth) with the integer representing the order in which you want the elements to appear. (e.g. `flex-1-sm`, will be ordered as first element on 'small' screens (below 480px). 

Because of the support of Flexbox you can also use all other features, such as `align-self`, `justify-content` and `flex-direction`.


