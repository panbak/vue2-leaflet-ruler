<script>
import { OptionsMixin, ControlMixin, optionsMerger } from "vue2-leaflet";
import "./leaflet-ruler/src/leaflet-ruler.js";
import "./leaflet-ruler/src/leaflet-ruler.css";
import L from "leaflet";

export default {
  name: "LRuler",
  mixins: [ControlMixin, OptionsMixin],
  mounted() {
    const options = optionsMerger(
      {
        ...this.controlOptions,
        options: this.options,
      },
      this
    );
    L.control.ruler(options).addTo(this.$parent.mapObject);
  },
  render() {
    return null;
  },
};
</script>