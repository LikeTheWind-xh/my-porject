<template>
	<view class="home_me">
		<view class="home">
			<button style="background-image: url(@/static/common/home.png);"></button>
			<text>首页</text>
		</view>
		<view class="me">
			<button  style="background-image: url(../../static/activa/logo.png);background-color:#53DC9C;"></button>
			<text>我的</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		}
	}
</script>

<style lang="scss">
.home_me {
	width: 100%;
	position: absolute;
	height: 150rpx;
	bottom: 0;
	border-top: 1rpx solid #BFBFBF;
	display: flex;
	justify-content: space-between;

	view {
		width: 200rpx;
		display: flex;
		flex-direction: column;
		align-items: center;
		button {
			margin-top: 10rpx;
			width: 100rpx;
			background-position: center;
			background-size: 20px 20px;
			height: 100rpx;
			// background-color: #D4D4D4;
			background-repeat: no-repeat;
			background-image: url(../../static/common/home.png);
			border-radius: 40%;
		}
	}
}
</style>
