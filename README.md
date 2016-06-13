#Bootstrap 3 for IE7 (Beta)

[![Join the chat at https://gitter.im/coliff/bootstrap-ie7](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/coliff/bootstrap-ie7?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Bootstrap 3 dropped support for Internet Explorer 7, but you can add it back by simply adding this conditional CSS.

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

* Q. Does this include the new Glyphicons introduced in Bootstrap 3.3.2?

  A. Yep!

* Q. What about rounded corners, box shadows and gradients for IE7. How can I get those? 

  A. I recommend CCS3Pie for adding support for those CSS3 properties to older IE. http://css3pie.com/. 
     If you use that you can add this to your CSS to quickly add border-radius https://gist.github.com/coliff/5618329

* Q. What about Internet Explorer 6?

  A. Although this CSS does not include IE6-specific fixes, it does fix the webfonts icon, so it's worthwhile using the conditional code 'if lt IE 8' rather than 'if IE 7'.

* Q. What about Boostrap 4?
 
  A. I'm working on a new CSS file to add Internet Explorer 8 support to Bootstrap 4. Check it out at: https://github.com/coliff/bootstrap-ie8

### Known Issues
- The boxsizing.htc polyfill can be  a little bit buggy. Please make sure you follow the instructions for using that carefully.
- As this is only a CSS stylesheet there may be problems with using Bootstrap 3's JavaScript in IE7.
- Please open a pull request If you've fixed something.

<a href='http://ko-fi.com?i=1295NGMK1L2T7' target='_blank'><img style='border:0px;width:180px;' src='https://az743702.vo.msecnd.net/cdn/btn1.png' border='0' alt='Buy me a coffee at ko-fi.com'></a> 
