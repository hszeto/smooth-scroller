# smooth_scroller.js
___   
Allows pages to scroll up and down at predefined speed using Javascript and jQuery.
___
#### How it works:
smooth_scroller.js will listen for click events on the navbar. (nav tag is required).   
The href's on each navbar tab points to an id. The script will scroll to the div with the id at predefined speed.   
Much better UX!
___
#### Usage:
1. Add script tag for jQuery in the html head.
2. Add script tag for smooth_scroller.js in html head. (after jQuery)
3. Use '$SS' to define smooth_scroller. 

##### Example:
###### In index.html:
```
  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
  
  <div id="home">Home</div>
  <div id="contact">Contact</div>
```
###### In javascript file: 
 ```javascript
$(document).ready(function(){
  $SS().start(3000);
})
 ```
___
###### Option:
The scroll speed (millisecond) can be defined in start. If left empty, default speed is 1000ms.
###### Example: (no quote around the number)
 ```javascript
$SS().start(3000);
 ```
___
#### Demo:  
Visit https://jsfiddle.net/hszeto/Lgy2cg5a/
