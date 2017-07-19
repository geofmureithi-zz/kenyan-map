# Kenyan Map
Kenyan Map with Counties in svg Format and also in D3.js 

## Synopsis
I created this repo, despite its **unconventional** nature (I could have created gists) to assist me and anyone else looking to work with the Kenyan Map
The examples in this repo are using
- **D3v4**
- **D3 multi-selection**

The React example additionally incoporates:
- **React FauxDOM**

The examples here assume you are familiar with ES6;

## Usage 

### D3.js

```javascript
//see examples/D3.js
var mapCanvas = d3.select(selection).attrs({
      "xmlns:dc": "http://purl.org/dc/elements/1.1/",
      "xmlns:cc": "http://creativecommons.org/ns#",
      "xmlns:rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
      "xmlns:svg": "http://www.w3.org/2000/svg",
      "xmlns": "http://www.w3.org/2000/svg",
      "version": "1.2",
      "width": "100%",
      "height": "100%",
      "viewBox": "0 0 800 700",
      "id": "svgmapid",
      "style": "fill:none;stroke:#000000;stroke-width:1"
});
var metadata = mapCanvas.append('metadata').attrs({
   "id": "kenyanMap"
});
//......
```
### Angular V1.5 +
Angular v1.5 introduced **components** via `.component`.
```javascript
//see examples/AngularV1.js
//copy the file to something like kenyanmap.component.js
let mapModule = angular.module('app.kenyanMap', []);
import kenyanMapComponent from './kenyanmap.component'
mapModule.component('kenyanMap', kenyanMapComponent);
```

### React
See example usage [here](https://github.com/geofmureithi/254-Election-Predictor/blob/master/src/components/DrawMap.js)
```javascript
//see examples/React.js
//copy the file to something like KenyanMap.js
//Improve on it by using props
import KenyanMap from './KenyanMap';

const MapWrapper = (props) => {
  return(<KenyanMap />)
}
```
## Contributions
Feel free to create PRs of your improvements or usage.

## Licence
MIT


