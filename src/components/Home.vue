<template>
	<div class="Home">
		<el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
			
		</el-menu>
	</div>
</template>
<script>
import axios from "axios";
export default {
	name: "Home",
	components: {

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

	.el-menu {
		 background-color: rgba(255,255,255,0) !important;
	}
	.el-menu.el-menu--horizontal {
		border-bottom: none !important;
	}
	.el-row {
		margin-bottom: 20px;
		&:last-child {
      		margin-bottom: 0;
    	}	
  	}
  	.el-col {
    	border-radius: 4px;
  	}
  	.bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }

</style>