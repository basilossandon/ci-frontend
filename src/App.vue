<template>
  <div id="app">
    <Svg/>
  </div>
</template>

<script>
import Svg from "./components/Svg.vue";
export default {
  name: "app",
  components: {
    Svg
  },
  data() {
    return {};
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>