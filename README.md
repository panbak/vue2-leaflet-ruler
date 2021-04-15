# vue2-leaflet-ruler
a Vue2Leaflet plugin wrapper for [leaflet-ruler](https://github.com/gokertanrisever/leaflet-ruler)

##Installation
`npm install --save panbak/vue2-leaflet-ruler`

##Usage
`
//...
import LRuler from "vue2-leaflet-ruler";
//...

export default {
  //...
  components: {
    "l-ruler": LRuler,
  },
  //...
`

At the moment only default options of [leaflet-ruler](https://github.com/gokertanrisever/leaflet-ruler) are supported.

`
<l-map>
  <!-- other components -->
  <l-ruler />
</l-map>
`

##Credits
Thanks to the contributors of the [leaflet-ruler](https://github.com/gokertanrisever/leaflet-ruler) plugin.

##Author
Panagiotis Bakas

##License
This project is licensed under the MIT License .
