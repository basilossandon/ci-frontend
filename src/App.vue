<template>
  <div id="app">
    <Home/>
  </div>
</template>

<script>
import Home from "./components/Home.vue";
import Products from "./components/Products.vue";
export default {
  name: "app",
  components: {
    Home,
    Products
  },
  data() {
    return {};
  }
};
</script>

<style>
*{
  margin: 0px !important;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>