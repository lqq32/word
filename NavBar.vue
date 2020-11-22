<template>
	<!-- 导航条 -->
	<div class="bj">       <!-- 背景 -->
		<div class="wenz">      <!-- 模型盒子 -->
			<ul class="menu" >    <!-- 列表菜单 -->
				<li><span>首页</span></li>
				<li><span id="gs" @mouseenter="Mouseenter()" @mouseleave="Mouseleave()">菜品</span>
				<div class="dropdown" id="one">
					<ul class="fenl" >    <!-- 列表菜单 -->
						<li><span>中式菜品</span></li>
						<li><span>西式菜品</span></li>
						<li><span>饮品</span></li>
					</ul>
				</div>
				</li>
				<li><span id="dj">餐厅文化</span>
				<div class="dropdown" id="two">
					<ul class="fenl" >    <!-- 列表菜单 -->
						<li><span>美食</span></li>
						<li><span>休闲娱乐</span></li>
						<li><span>伴手礼</span></li>
					</ul>
				</div>
				</li>
				<!-- <li><span id="wh">文化乌镇</span> -->
				<!-- <div class="dropdown" id="three"> -->
					<!-- <ul class="fenl" >     列表菜单 -->
						<!-- <li><span>乌镇戏剧节</span></li> -->
						<!-- <li><span>艺术邀请展</span></li> -->
					<!-- </ul> -->
				<!-- </div> -->
				<!-- </li> -->
				<!-- <li><span id="hz">会展乌镇</span> -->
				<!-- <div class="dropdown" id="four"> -->
					<!-- <ul class="fenl" >    列表菜单 -->
						<!-- <li><span>服务介绍</span></li> -->
						<!-- <li><span>成功案例</span></li> -->
					<!-- </ul> -->
				<!-- </div> -->
				<!-- </li> -->
				<!-- <li><span>互动体验</span></li> -->
				<li><span id="hd">活动广告</span>
				<div class="dropdown" id="five">
					<ul class="fenl" >    <!-- 列表菜单 -->
						<li><span>景区活动</span></li>
						<li><span>新闻动态</span></li>
					</ul>
				</div>
				</li>
				<li><span>联系我们</span></li>
				<li><span>关于我们</span></li>
			</ul>
			<!-- 列表下的分类 -->
			
		</div>
	</div>
</template>

<script>
	export default {
		
	}
</script>

<style>
	.bj{
		width: 100%;
		height: 60px;
		/* background: #53577F; */
		background-color: rgba(128,138,135);
		cursor: pointer;
		position: relative;
	}
	.wenz{
		width: 1200px;
		z-index: 2.5;
		margin-left:auto;
		margin-right: auto;
		
	}
	.wenz .menu{
		color: #FFFFFF;
		list-style-type: none;
		margin-left: 600px;
	}
	.wenz .menu li{
		float: left;
		padding: 1.6em 1.2em;
		line-height: 1.5em;
		margin-right: 10px;
		/* color: #FFFFFF; */
	}
	.wenz .menu  li span{
		font-size: 15px;
	}
	.dropdown {
		position: absolute;
		width: 130px;
		height: 90px;
		line-height: 5px;
		padding: auto;
		background-color: rgba(128,138,135);
		display: none;
	}
	.fenl {
		color: #FFFFFF;
		list-style-type: none;
		padding: 1em 1em;
		font-size: 12px;
	}
	.wenz .menu .dropdown li{
		margin-top: -.5em;
		margin-bottom: -.8em;
	}
	.wenz .menu .dropdown li:hover{
		background: black;
	}
	.wenz .dropdown.open {
		display: block;
		
	}
</style>