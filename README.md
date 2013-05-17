jquery-dim-background
=====================

jQuery plugin to dim the current page except for some user-defined top elements.


Usage
-----

Include the script in your website first. Add this script tag after your jQuery inclusion.

```html
<script type="text/javascript" src="https://raw.github.com/andywer/jquery-dim-background/master/lib/jquery.dim-background.js"></script>
```


Usage is simple. You can dim your website, but keep some elements on top of the curtain:

```html
<script type="text/javascript">
    $('.myElements').dim();
</script>
```


To switch back to normal:

```html
<script type="text/javascript">
    $('.myElements').undim();
    // - or -
    $.undim();
</script>
```


You can also provide a callback function that is called when the animation completes and you can overwrite default options:

(You may find the available options in the `jquery.dim-background.js` file. Have a look at `$.fn.dimBackground.defaults`)

```html
<script type="text/javascript">
    $('.myElements').dim({
        darkness : 0.8            // 0: no dimming, 1: completely black
    }, function() {
        // do something
    });
</script>
```


Have a lot of fun!
