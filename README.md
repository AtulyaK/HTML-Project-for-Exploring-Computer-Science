# HTML-Project-for-Exploring-Computer-Science
This is a project I did in my Exploring Computer Science Class.

I had put 5 pages for the project. 

1. There are two pages that were not complete at the time.
  
	a. One of the pages had a trial page. That is labeled as **trialpage2.html**. This page had an extremely cool search feature. It allowed you to search for a 
     name of a car brands, drivetrain types, exterior color, and interior color. **The search function works properly**.
  
	b. The second page was not completed.

2. The other 3 pages work fine.

# I also want to give credits to Dynamic Drive for some of the features like the navigation bar and a scroller


# Below is the TouchSwipe 1.6 ReadMe.md

# TouchSwipe 1.6
A jQuery plugin to be used on touch devices such as iPad, iPhone, Android etc.

Detects single and multiple finger swipes, pinches and falls back to mouse 'drags' on the desktop.

Time and distance thresholds can be set to distinguish between swipe gesture and slow drag.

Allows exclusion of child elements (interactive elements) as well allowing page scrolling or page zooming depending on configuration.

* Detects swipes in 4 directions, "up", "down", "left" and "right"
* Detects pinches "in" and "out"
* Supports single finger or double finger touch events
* Supports click events both on the touchSwipe object and its child objects
* Definable threshold / maxTimeThreshold to determin when a gesture is actually a swipe
* Events triggered for swipe "start","move","end" and "cancel"
* End event can be triggered either on touch release, or as soon as threshold is met
* Allows swiping and page scrolling
* Disables user input elements (Button, form, text etc) from triggering swipes

## Demos, examples and docs

[http://labs.rampinteractive.co.uk/touchSwipe](http://labs.rampinteractive.co.uk/touchSwipe)  
[http://labs.rampinteractive.co.uk/touchSwipe/docs](http://labs.rampinteractive.co.uk/touchSwipe/docs)


## Installation  
### NPM
````bash
npm install jquery-touchswipe --save
````
### Bower
````bash
bower install jquery-touchswipe --save
````
### Manual
Include the minified file in your project.
````html
<script type="text/javascript" src="js/jquery.touchSwipe.min.js"></script>
````

## Usage
````javascript
$(function() {
  $("#test").swipe( {
    //Generic swipe handler for all directions
    swipe:function(event, direction, distance, duration, fingerCount, fingerData) {
      $(this).text("You swiped " + direction );  
    }
  });

  //Set some options later
  $("#test").swipe( {fingers:2} );
});
````

For full demos, code examples and documentation, see below.


## Development
Install dependencies
````bash
npm install
````

To minify
````bash
npm run minify
````

To build docs
````bash
npm run docs
````

To do both
````bash
npm run build
 ````

### For port to XUI see:
https://github.com/cowgp/xui-touchSwipe
