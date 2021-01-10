# Chart.js, Canvas

## Chart.js

#### `<canvas>`: use to render the chart.

#### `<canvas>` looks like the <img> element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the <canvas> element has only two attributes, width and height. 

#### `<script src="https://cdn.jsdelivr.net/npm/chart.js@2.8.0"></script>` is use to include Chart.js in our page, or we can use ` <script src='Chart.min.js'></script>`.


#### Example:
```
<canvas id="myChart" width="400" height="400"></canvas>
<script>
var ctx = document.getElementById('myChart').getContext('2d');
var myChart = new Chart(ctx, {
    type: 'bar',
    data: {
        labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
        datasets: [{
            label: '# of Votes',
            data: [12, 19, 3, 5, 2, 3],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        scales: {
            yAxes: [{
                ticks: {
                    beginAtZero: true
                }
            }]
        }
    }
});
</script>
```

#### The `fillRect()` function draws a large black square 100 pixels on each side. The `clearRect()` function then erases a 60x60 pixel square from the center, and then `strokeRect()` is called to create a rectangular outline 50x50 pixels within the cleared square.

### Colors:

#### fillStyle = color
* Sets the style used when filling shapes.
#### strokeStyle = color
* Sets the style for shapes' outlines.

#### color is a string representing a CSS `<color>`, a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).

#### Line styles
  There are several properties which allow us to style lines. 

* lineWidth = value
  Sets the width of lines drawn in the future.
* lineCap = type
  Sets the appearance of the ends of lines.
* lineJoin = type
  Sets the appearance of the "corners" where lines meet.
* miterLimit = value
  Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
* getLineDash()
  Returns the current line dash pattern array containing an even number of non-negative numbers.
* setLineDash(segments)
  Sets the current line dash pattern.
* lineDashOffset = value
  Specifies where to start a dash array on a line.

#### Exmple:
```
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  for (var i = 0; i < 10; i++) {
    ctx.lineWidth = 1 + i;
    ctx.beginPath();
    ctx.moveTo(5 + i * 14, 5);
    ctx.lineTo(5 + i * 14, 140);
    ctx.stroke();
  }
}
```

### Drawing text:

* fillText(text, x, y [, maxWidth])
   Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
* strokeText(text, x, y [, maxWidth])
  Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.