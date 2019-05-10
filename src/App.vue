<template>
	<div id="app">
		<Svg/>
	</div>
</template>
<script>
import axios from "axios";
import Svg from './component/Svg.vue';

export default {
	name: "app",
	components: {
		Svg
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
		margin-top: 60px;
	}
</style>