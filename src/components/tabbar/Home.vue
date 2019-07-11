<template>
	<div>
		<mt-swipe :auto="4000">
			<mt-swipe-item>1</mt-swipe-item>
			<mt-swipe-item>2</mt-swipe-item>
			<mt-swipe-item>3</mt-swipe-item>
		</mt-swipe>
	</div>
</template>

<script>
	export default {
		data(){
			return{}
		},
		created(){
			this.getLunBo();
		},
		methods: {
			getLunBo(){
				this.$http.get("http://vue.studyit.io/api/getlubo").then(reuslt =>{
					console.log(result);
				})
//				$.ajax({
//					type:"GET",
//					url:"http://vue.studyit.io/api/getlubo",
//					dataType: "JSON",
//					success:function(data){
//						console.log(data.body)
//					}
//				})
			}
		}
	}
</script>

<style scoped lang="scss">
	.mint-swipe{
		height: 200px;
		
	}
	.mint-swipe-item{
		background-color: lightcyan;
	}
</style>