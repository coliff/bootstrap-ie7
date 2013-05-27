#Bootstrap 3 for IE7 (Beta)

Bootstrap is awesome for getting your webapp started. With Bootstrap 3 support for Internet Explorer 7 has been dropped. If you need support for IE7 simply add this CSS script and support will be reinstated.

##FAQS

Q. Do I need to make any changes to my HTML to add support for bootstrap3-ie7?  
A. The only change you need to make is adding a class glyphicon-white to any icons you wish to be white. If you don't add this class then icons will be dark grey. Unlike the webfont icons, no other colours are available for bootstrap3-ie7 as it uses a PNG sprite.

Q. What about rounded corners, box shadows and gradients for IE7. How can I get those?
A. I recommend CCS3Pie for adding support for those CSS3 properties to older IE. http://css3pie.com/

Q. Bootstrap 3 also drops support for -webkit and -moz prefixes for border-radius and box shadows. Will you re-add support for those browsers too?  
A. I recommend http://leaverou.github.com/prefixfree/ to automatically add support for Firefox 3.6 and Safari 4, iOS 3.2 etc.


##Known Issues
- This is NOT ready for use yet. I'm working on a big update to match the latest Bootstrap 3 CSS changes. 
- Boostrap 3 uses the box-sizing property for layouts which is not supported by IE7. I recommend a polyfill https://github.com/Schepp/box-sizing-polyfill
- Due to the fact that the Glyphicon fallback uses a fixed-size sprite image, icons can only be displayed in one size
