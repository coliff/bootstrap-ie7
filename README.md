#Bootstrap 3 for IE7 (Beta)

Bootstrap 3 drops support for Internet Explorer 7, but you can add it back by simply adding this conditional CSS.

```html
<!--[if lt IE 8]>
    <link href="/css/bootstrap-ie7.css" rel="stylesheet">
<![endif]-->
```

### Requirements
- Bootstrap 3 uses the box-sizing property for layouts which is not natively supported by IE7. The polyfill 'boxsizing.htc' is required: https://github.com/Schepp/box-sizing-polyfill


### FAQS

* Q. Do I need to make any changes to my HTML to add support for bootstrap3-ie7? 

  A. Nope! Just include the conditional IE7 stylesheet and you're ready to go!


* Q. What about rounded corners, box shadows and gradients for IE7. How can I get those? 

  A. I recommend CCS3Pie for adding support for those CSS3 properties to older IE. http://css3pie.com/. 
     If you use that you can add this to your CSS to quickly add border-radius https://gist.github.com/coliff/5618329

* Q. What about Internet Explorer 6?

  A. Although this CSS does not include IE6-specific fixes, it does fix the webfonts icon, so it's worthwhile using the conditional code 'if lt IE 8' rather than 'if IE 7'.


### Known Issues
- This is not complete yet. I'm working on fixing some issues to match the final Bootstrap 3.2 CSS changes. Please open a pull request If you've fixed something.
- The boxsizing.htc polyfill is buggy and generally doesn't work very well. I'm looking at refactoring the grids CSS to match Bootstrap 2.x so that the polyfill is not required.
- As this is only a CSS stylesheet there may be problems with using Bootstrap 3's JavaScript in IE7.
