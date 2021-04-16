# vue2-leaflet-ruler
a Vue2Leaflet plugin wrapper for [leaflet-ruler](https://github.com/gokertanrisever/leaflet-ruler)

## Installation

`npm i vue2-leaflet-ruler`

## Usage

```
//...
import LRuler from "vue2-leaflet-ruler";
//...

export default {
  //...
  components: {
    "l-ruler": LRuler,
  },
  //...
```

At the moment only default options of [leaflet-ruler](https://github.com/gokertanrisever/leaflet-ruler) are supported.

```
<l-map>
  <!-- other components -->
  <l-ruler :options="rulerOptions" />
</l-map>
```

Available options (These are the default)

```
rulerOptions: {
        position: "topright", // Leaflet control position option
        circleMarker: {
          // Leaflet circle marker options for points used in this plugin
          color: "red",
          radius: 2,
        },
        lineStyle: {
          // Leaflet polyline options for lines used in this plugin
          color: "red",
          dashArray: "1,6",
        },
        lengthUnit: {
          // You can use custom length units. Default unit is kilometers.
          display: "km", // This is the display value will be shown on the screen. Example: 'meters'
          decimal: 2, // Distance result will be fixed to this value.
          factor: null, // This value will be used to convert from kilometers. Example: 1000 (from kilometers to meters)
          label: "Distance:",
        },
        angleUnit: {
          display: "&deg;", // This is the display value will be shown on the screen. Example: 'Gradian'
          decimal: 2, // Bearing result will be fixed to this value.
          factor: null, // This option is required to customize angle unit. Specify solid angle value for angle unit. Example: 400 (for gradian).
          label: "Bearing:",
        },
      },

```

## Credits

Thanks to the contributors of the [leaflet-ruler](https://github.com/gokertanrisever/leaflet-ruler) plugin.

## Author

Panagiotis Bakas

## License

This project is licensed under the MIT License .
