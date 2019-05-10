<template>
  <div class="Home">
    <!-- <el-menu
      :default-active="activeIndex"
      class="el-menu-demo"
      mode="horizontal"
      @select="handleSelect"
    >
    </el-menu> -->
	 <el-button round plain v-on:click="getAxios()">Axios</el-button>
  </div>
</template>
<script>
import axios from "axios";
export default {
  name: "Home",
  data() {
	  return {
	  }
  },
  components: {

  },
  methods:{
	  getAxios() {
		  axios.get("http://157.230.12.110:8080/productos/productoes").then(
			  (response) => {
				  console.log(response.data)
				  console.log("Ready")
			  }
		  );
	  }
  }
};
</script>
<style>
.Home {
  background: url(../assets/background.svg) no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  height: 100vh;
  width: 100%;
}
</style>