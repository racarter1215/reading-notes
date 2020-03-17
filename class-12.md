# Basic Usage

### The canvas element

##### <canvas id="tutorial" width="150" height="150"></canvas>

##### similar to image code but doesn't have src or alt attributes. without width or height defined, it is set at 300px width and 150px high.

##### The <canvas> element differs from an <img> tag in that, like for <video>, <audio>, or <picture> elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.
  
##### Canvas REQUIRES a closing /canvas tag. Also, if the browser doesn't read canvas, you can always add image/alt information within the code

##### The fallback content is displayed in browsers which do not support <canvas>. Scripts can also check for support programmatically by simply testing for the presence of the getContext() method. Our code snippet from above becomes something like this:

var canvas = document.getElementById('tutorial');

if (canvas.getContext) {
  var ctx = canvas.getContext('2d');
  // drawing code here
} else {
  // canvas-unsupported code here
}

##### A skeleton template
Here is a minimalistic template, which we'll be using as a starting point for later examples.

Note: it is not good practice to embed a script inside HTML. We do it here to keep the example concise.

### !DOCTYPE html>
##### html>
  <head>
    <meta charset="utf-8"/>
    <title>Canvas tutorial</title>
    <script type="text/javascript">
      function draw() {
        var canvas = document.getElementById('tutorial');
        if (canvas.getContext) {
          var ctx = canvas.getContext('2d');
        }
      }
    </script>
    <style type="text/css">
      canvas { border: 1px solid black; }
    </style>
  </head>
  <body onload="draw();">
    <canvas id="tutorial" width="150" height="150"></canvas>
  </body>
</html>

### Drawing Shapes

##### The grid
Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can translate the origin to a different position, rotate the grid and even scale it, but for now we'll stick to the default.


