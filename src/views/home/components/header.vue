<template>
	<div class="header">
		<div class="header-left"><i class="iconfont">&#xe624;</i></div>
		<div class="header-input">输入内容</div>
		<div class="header-right">城市 <i class="iconfont">&#xe62d;</i></div>
	</div>
</template>

<script>

export default {
  name: 'HomeHeader'
}
</script>

<style scoped>
.header {
	display: flex;
	line-height: 0.86rem;
	background-color: #bdc4bc;
	color: white;
}
.header-left {
	width: 0.64rem;
	float: left;
}
.header-input {
	flex: 1;
	height: 0.64rem;
	background-color: white;
	border-radius: 0.1rem;
	margin-top: 0.12rem;
	margin-left: 0.12rem;
	color: grey;
}
.header-right {
	width: 1.24rem;
	float: right;
	text-align: center;
}

	
</style>