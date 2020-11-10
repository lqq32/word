<template>
	<!-- 1楼：顶部条 -->
	<div class="topbar">
		<div class="container">
			<a href="#">
				<span class="fa fa-star"></span>
				收藏i前端
			</a>
			<a href="#">
				<span class="fa fa-mobile-phone fa-lg"></span>
				<span class="theme-reverse">下载手机客户端</span>
			</a>
			<span>
				<span class="fa fa-envelope"></span>
				反馈邮箱：iweb@tedu.cn
			</span>
			<span>
				<span class="fa fa-mobile-phone fa-lg"></span>
				客服热线：4008-200-200
			</span>
		</div>
	</div>
</template>

<script>
	export default{
		
	}
</script>

<style>
	.topbar {
		width: 100%;
		height: 29px;
		line-height: 29px;
		background: #f9f9f9;
		border-bottom: 1px solid #eee;
		text-align: right;
	}
	.container {
		width: 1000px;
		margin-left: auto;
		margin-right: auto;
		border: 1px solid #aaa;	/*仅供测试用*/
	}
	.topbar > .container > a,
	.topbar > .container > span {	/*复杂选择器：> 选择孩子，逗号表示并列选多个*/
		padding-left: 1em;
	}
	.theme {			/*主题色*/
	}
	.theme-reverse {	/*主题色的反色*/
		color: #f60;	
	}
</style>