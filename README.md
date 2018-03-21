

# ChartJS

> npm install
> npm install -g gulp

> gulp build                // build Chart.js in ./dist
> gulp unittest             // run tests from ./test/specs
> gulp unittest --watch     // run tests and watch for source changes
> gulp unittest --coverage  // run tests and generate coverage reports in ./coverage
> gulp lint                 // perform code linting (ESLint)
> gulp test                 // perform code linting and run unit tests
> gulp docs                 // build the documentation in ./dist/docs


<canvas id="myChart"></canvas>

<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.4.0/Chart.min.js"></script>

var ctx = document.getElementById('myChart').getContext('2d');
var chart = new Chart(ctx, {
    // The type of chart we want to create
    type: 'line',

    // The data for our dataset
    data: {
        labels: ["January", "February", "March", "April", "May", "June", "July"],
        datasets: [{
            label: "My First dataset",
            backgroundColor: 'rgb(255, 99, 132)',
            borderColor: 'rgb(255, 99, 132)',
            data: [0, 10, 5, 2, 20, 30, 45],
        }]
    },

    // Configuration options go here
    options: {}
});

