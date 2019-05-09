<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Hola Gabriel"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import axios from "axios"

export default {
  name: 'app',
  components: {
    HelloWorld
  },

  craeted() {
    console.log('Axios');
    axios.get("http://157.230.12.110:8080/productos").then(
      (response) => {
        console.log(response.data);
        console.log('AXIOS READY')
      }
    );
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
