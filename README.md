# Finite-Reports
Slick reporting capabilities for the [FiniteJS](https://github.com/rkuzsma/finite) integration test library.

## Getting Started

`npm install --save-dev finite-reports`

example.html
```html
<html>
  <script language="javascript" src="require.js">
  <script language="javascript" src="finite.js">
  <script language="javascript" src="finite-reports.js">
  <body>
    <div id="reportsDiv"/>
  </body>
  <script language="javascript">
    var Finite = require('finite');
    var FiniteReports = require('finite-reports');

    // Load your FiniteJS test plan directly...
    var plan = { name: "My Test Plan" };
    // Or load plan from some updatable JSON resource URL.

    FiniteReports.load(plan, 'reportsDiv');

    // Run the plan. Finite-Reports will auto-refresh.
    Finite.run(plan);
  </script>
</html>
```


## API

* `load(plan, el)`: Load the Finite-Reports reporting UI into the specified HTML element.

## Screenshots
