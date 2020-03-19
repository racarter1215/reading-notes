# Transform Property

### div {
###   -webkit-transform: scale(1.5);
###      -moz-transform: scale(1.5);
###        -o-transform: scale(1.5);
###           transform: scale(1.5);

### 2D Transforms

##### Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth. We’ll start by discussing how to transform elements on a two-dimensional plane, and then work our way into three-dimensional transforms.

### 2D Rotate

##### The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. Later we will discuss how you can change this default point of rotation.

##### <figure class="box-1">Box 1</figure>
##### <figure class="box-2">Box 2</figure>
##### .box-1 {
#####   transform: rotate(20deg);
##### }
##### .box-2 {
#####   transform: rotate(-55deg);
##### }

### 2D Scale

##### Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.

##### <figure class="box-1">Box 1</figure>
##### <figure class="box-2">Box 2</figure>

##### .box-1 {
#####   transform: scale(.75);
##### }
##### .box-2 {
#####   transform: scale(1.25);
##### }

##### It is possible to scale only the height or width of an element using the scaleX and scaleY values.

##### <figure class="box-2">Box 2</figure>
##### <figure class="box-3">Box 3</figure>

##### .box-1 {
#####   transform: scaleX(.5);
##### }
##### .box-2 {
#####   transform: scaleY(1.15);
##### }
##### .box-3 {
#####   transform: scale(.5, 1.15);
##### }

### 2D Translate

##### The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.

##### As with the scale value, to set both the x and y axis values at once, use the translate value and declare the x axis value first, followed by a comma, and then the y axis value.

##### The distance values used within the translate value may be any general length measurement, most commonly pixels or percentages. Positive values will push an element down and to the right of its default position while negative values will pull an element up and to the left of its default position.

##### <figure class="box-1">Box 1</figure>
##### <figure class="box-2">Box 2</figure>
##### <figure class="box-3">Box 3</figure>

##### .box-1 {
#####   transform: translateX(-10px);
##### }
##### .box-2 {
#####   transform: translateY(25%);
##### }
##### .box-3 {
#####   transform: translate(-10px, 25%);
##### }

# Find all additional types of code at https://learn.shayhowe.com/advanced-html-css/css-transforms/

### 8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS

##### <!DOCTYPE html>
##### <html>
##### <head>
#####     <style type="text/css">
#####     </style>
##### </head>
##### <body>
#####   <div></div>
##### </body>
##### </html>

#####  <style type="text/css">
#####  body > div
#####  {
#####              width:483px;
#####              height:298px;
#####              background:#676470;
#####              transition:all 0.3s ease;
##### }
#####  </style>

##### Fade In:
##### Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover:

##### .fade
##### {
#####         opacity:0.5;
##### }
##### .fade:hover
##### {
#####         opacity:1;
##### }

##### Change color
##### Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values ##### and then recombining them. Now, we just set the div’s class to “color” and specify the color we want in our CSS:

##### .color:hover
##### {
#####         background:#53a7ea;
##### }

##### Grow & Shrink
##### Set your div’s class to “grow” and then add this code to your style block:

##### .grow:hover
##### {
#####         -webkit-transform: scale(1.3);
#####         -ms-transform: scale(1.3);
#####         transform: scale(1.3);
##### }

##### The rest of these simle tricks are found at: https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users/.

