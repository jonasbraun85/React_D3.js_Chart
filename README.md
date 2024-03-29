## react-d3
Modular ReactJS charts made using d3 chart utilities. Work on project documentation has started [here](https://github.com/esbullington/react-d3/wiki). A few examples of the available charts can be seen below, the others can be [viewed here](https://reactiva.github.io/react-d3-website/), side-by-side with the React code that generates the charts.

![react-d3 chart images](https://raw.githubusercontent.com/esbullington/react-d3-website/gh-pages/img/multiseries.png)

[![Build Status](https://travis-ci.org/esbullington/react-d3.svg?branch=master)](https://travis-ci.org/esbullington/react-d3)

## Basic usage

First, install via `npm`:

`npm install react-d3`

Then, import into your ReactJS project:

```
var rd3 = require('react-d3');
// es6
import rd3 from 'react-d3';
```

The charts are then available under the `rd3` namespace, which you can then use as shown on the [demonstration page](https://reactiva.github.io/react-d3-website/):

```
var BarChart = require('react-d3/barchart').BarChart;
// es6
import { BarChart } from 'react-d3';
```

## Available Charts

```
var BarChart = rd3.BarChart;
var LineChart = rd3.LineChart;
var PieChart = rd3.PieChart;
var AreaChart = rd3.AreaChart;
var Treemap = rd3.Treemap;
var ScatterChart = rd3.ScatterChart;
var CandleStickChart = rd3.CandleStickChart;
```

For usage, please see [here](https://reactiva.github.io/react-d3-website/).  [API documentation](https://github.com/esbullington/react-d3/wiki/API) is also coming online over the coming days.

## JSFiddle
There's a development build available for experimentation on JSFiddle: [http://jsfiddle.net/esbullington/jp9dkh1g/](http://jsfiddle.net/esbullington/jp9dkh1g/).

Please note that this build should probably not be used in production, since it bundles all of react-d3's dependencies in a single bundle (this is also the cause of the "Cannot read property 'firstChild' of undefined" error message on the JS console, which occurs when there are two React libraries in the same namespace).

All the react-d3 charts are available in this JSFiddle fork under the global `rd3` namespace.
