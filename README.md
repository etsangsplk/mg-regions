# mg-regions

A metrics-graphics addon allowing region annotations for line charts.

### Usage

Install using bower (not yet published):

- `bower install senseye/mg-regions --save`

Include `dist/mg_regions.js` in your build, or include it in your HTML:

- `<script src="bower_components/mg_regions/dist/mg_regions.js"></script>`

Import the default styles from `dist/mg_regions.css`, or create your own:

- `<link rel="stylesheet" href="bower_components/mg_regions/dist/mg_regions.css" type="text/css" />`

Add regions to your line charts by specifing a regions argument in the chart options. This argument should contain an array of regions, each made up of an array specifing the start and end points and a label. For example, the following produces a region between 1994 and 2004 with a label 'friends':

```js
regions: [{
  date: [1994, 2004],
  label: 'friends'
}]
```

### Testing

- `gulp test` to run the Test'em server in continuous mode.
- `npm test` or `gulp test-ci` for a single run, CI mode.