#Bootstrap 3 for IE7 (Beta)

Bootstrap 3 drops support for Internet Explorer 7, but if you need support for IE7 simply add this conditional CSS and support will be reinstated.

##FAQS

Q. Do I need to make any changes to my HTML to add support for bootstrap3-ie7?  
A. The only change you need to make is adding a class glyphicon-white to any icons you wish to be white. If you don't add this class then icons will be dark grey. Unlike the webfont icons supplied with BS3, no other colours are available for bootstrap3-ie7 as it uses a PNG sprite.

Q. What about rounded corners, box shadows and gradients for IE7. How can I get those?
A. I recommend CCS3Pie for adding support for those CSS3 properties to older IE. http://css3pie.com/


##Known Issues
- This is not complete yet. I'm working on a big update to match the release Bootstrap 3 CSS changes. 
- Boostrap 3 uses the box-sizing property for layouts which is not supported by IE7. The polyfill is required: https://github.com/Schepp/box-sizing-polyfill
- Due to the fact that the Glyphicon fallback uses a fixed-size sprite image, icons can only be displayed in one size
