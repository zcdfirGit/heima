<template>
  <div class="divClass_box">
  	<mt-header fixed title="黑马项目"></mt-header>
   
    <router-view></router-view>
    <nav class="mui-bar mui-bar-tab">
			<router-link class="mui-tab-item " href="#tabbar" to="/home">
				<span class="mui-icon mui-icon-home"></span>
				<span class="mui-tab-label">首页</span>
			</router-link>
			<router-link class="mui-tab-item" href="#tabbar-with-meber" to="/member">
				<span class="mui-icon mui-icon-contact"></span>
				<span class="mui-tab-label">会员</span>
			</router-link>
			<router-link class="mui-tab-item" href="#tabbar-with-car" to="/shopcar">
				<span class="mui-icon mui-icon-extra mui-icon-extra-cart"><span class="mui-badge">0</span></span>
				<span class="mui-tab-label">购物车</span>
			</router-link>
			<router-link class="mui-tab-item" href="#tabbar-with-map" to="/search">
				<span class="mui-icon mui-icon-search"></span>
				<span class="mui-tab-label">搜索</span>
			</router-link>
		</nav>
  </div>
</template>

<script>
</script>


<style lang="scss" scoped>
	.divClass_box{
		padding-top: 40px;
	}
</style>
