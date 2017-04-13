# iOS7 style switch

[Check out the demo](http://wd.dizaina.net/en/experiments/ios7-style-switch/)

![iOS7 style switch](http://wd.dizaina.net/pics/ios7-style-switch/ios7-style-switch.png)

Features:

- no shitty scripts, pure CSS,
- the most accurate behavior, includes `:active` state styles,
- made with `em`s, sizes approprietaly to the font size,
- accessible from keyboard.

## Usage

Grab the css. Use it!

## Markup

```html
<label class="ios7-switch">
    <input type="checkbox" checked>
    <span></span>
</label>
```

or

```html
<label class="ios7-switch">
    <input type="checkbox" checked>
    <span></span>
    Mah shitty option!
</label>
```

or something else, you get the idea.

## Caveats

Doesn't work in older browsers with no `box-shadow` support (IE8 and lower, Android 3.x and lower). It's easy enough to make a fallback to regular checkboxes. For instance, using [Modernizr](http://modernizr.com) test

    Modernizr.addTest('unprefixed-boxshadow', Modernizr.testProp('boxShadow', '1px 1px', true));

and modified stylesheet -- [ios7-switch.modernizr.css](https://github.com/wilddeer/ios7-switch/blob/master/ios7-switch.modernizr.css).

Has some rounding error problems in some browsers at some font sizes. Tweak the font size a bit to get rid of those.

## License

You kiddin me, it's 100 rows of CSS, just use it already! Ok, here's some text for ya: [CC0 1.0](http://creativecommons.org/publicdomain/zero/1.0/). Shit, I'm so generous!
