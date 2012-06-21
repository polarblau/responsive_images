## jquery.responsive_images

*Use this with caution.* This plugin doesn't do anything fancy — I've
pretty much just thrown it together because most other solutions out
there do a lot more, name break points, check bandwidth etc. **This
plugin loads different images depending on the viewport size. That's
it.**

### Usage

Include jQuery and a jQuery debounce plugin (e.g. [diaspora/jquery-debounce](https://github.com/diaspora/jquery-debounce), then call this in a DOM-ready handler

```javascript
$('img.resposive').responsiveImages();
```

The plugin expects you define alternative versions through data attributes
according to the following pattern:

```javascript
// loads foo.jpg for screen width of 320 and up
data-320="path/to/images/foo.jpg"

// loads bar.jpg for screen width of 320 and up
data-480="path/to/images/bar.jpg"

...
```

Example:

```html
<img src="mobile.jpg" data-480="smartphone.jpg" alt="Description">
```
