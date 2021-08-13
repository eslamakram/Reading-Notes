# Docs for the HTML `<canvas>` Element & Chartjs

At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. the canvas will initially be 300 pixels wide and 150 pixels high.
The `<canvas>` element differs from an `<img>` tag in that, like for `<video>, <audio>, or <picture>` elements
The `<canvas>` element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown.

            var canvas = document.getElementById('tutorial');
               var ctx = canvas.getContext('2d')

Drawing shapes with canvas:

1. The grid
2. Drawing rectangles
3. Drawing paths
4. Drawing a triangle

   example:
             function draw() {
                var canvas = document.getElementById('canvas');
                if (canvas.getContext) {
                var ctx = canvas.getContext('2d');
                       ctx.beginPath();
                      ctx.moveTo(75, 50);
                      ctx.lineTo(100, 75);
                       ctx.lineTo(100, 25);
                       ctx.fill();
                                     }
                                   }
Creating a Chart
It's easy to get started with Chart.js. All that's required is the script included in your page along with a single `<canvas>` node to render the chart

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
            y: {
                beginAtZero: true
            }
        }
    }
     });
             </script>
