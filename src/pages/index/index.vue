<template>
	<view class="content">
		<image class="backgroundImage" src="../../static/home/background1.png"></image>
		<view class="rightTop">
			<navigator  url="../manual/manual">
				<view class="rightTopImage">
					<view class="rightTopText">
						<text>手动回收</text>
					</view>
					<image src="../../static/home/right.png"></image>
				</view>
			</navigator>
		</view>

		<view class="item">
			<image src="../../static/home/image.png"></image>
			<text>金阳光超市</text>
			<text>纯黄金<text style="font-size: 80rpx;font-weight: 800;">{{money}}</text>/斤</text>
		</view>

		<view class="foot">
			<view class="foot-button">
				<view class="button-border">
					<image src="../../static/home/border.png"></image>
				</view>

				<view class="button-content">
					<image src="../../static/home/boder-content.png"></image>
					<view class="button-text">
						<text>一键\n收纸</text>
					</view>
				</view>
			</view>
			<view class="phone">
				
				<button style="background-color: #28CD80;">{{mobile}}</button>
				<image src="../../static/home/phone.png"></image>
			</view>
			
			<view class="home_me">
				<view class="home">
					<button style="background-image: url(../../static/home/home.png);"></image></button>
					<text>首页</text>
				</view>
				<view class="me">
					<button style="background-image: url(../../static/home/me.png);"></button>
					<text>我的</text>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				money: 0.52,
				mobile:13215874691
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.backgroundImage {
		position: fixed;
		width: 100%;
		height: 100%;
		top: 0;
		left: 0;
		z-index: -1;
	}
	
	.rightTop {
		width: 100%;
	}
	
	.rightTopImage {
		image {
			width: 250rpx;
			height: 110rpx;
		}
	
		top: 20rpx;
		position: absolute;
		right: 0;
	
	}
	
	.rightTopText {
		position: absolute;
		right: 50rpx;
		top: 25rpx;
		z-index: 10;
		font-size: 26rpx;
		font-weight: 700;
		color: white;
	}
	
	.item {
		width: 100%;
		position: absolute;
		display: flex;
		flex-direction: column;
		align-items: center;
		top: 13%;
	
		image {
			width: 600rpx;
			height: 300rpx;
		}
	
		text {
			margin-top: 10rpx;
			color: #0b9f5a;
		}
	}
	
	.button-content,
	.button-border {
		position: absolute;
		top: 49%;
		margin: 0 auto;
		left: 23%;
	}
	
	.button-border image {
		width: 450rpx;
		height: 450rpx;
	}
	
	.button-content image {
		width: 300rpx;
		height: 300rpx;
		margin-top: 50rpx;
		margin-left: 60rpx;
	}
	
	.button-content .button-text {
		position: absolute;
		top: 30%;
		left: 40%;
		font-size: 60rpx;
		color: #1aa664;
		font-weight: 900;
	}
	
	.phone {
		width: 100%;
		position: absolute;
		top: 80%;
	
		image {
			position: absolute;
			width: 40rpx;
			height: 40rpx;
			left: 30%;
			top: 22rpx;
		}
	
		button {
			width: 45%;
			height: 80rpx;
			
			border-radius: 50rpx;
			border: 1rpx solid white;
			color: white;
			text-align: center;
			padding-left: 70rpx;
			line-height: 80rpx;
			margin: 0 auto;
	
		}
	}
	
	.home_me {
		width: 100%;
		position: absolute;
		height: 150rpx;
		bottom: 40rpx;
	
		display: flex;
		justify-content: space-between;
	
		view {
			width: 200rpx;
			display: flex;
			flex-direction: column;
			align-items: center;
			color: white;
			button {
				margin-top: 10rpx;
				width: 100rpx;
				background-position: center;
				background-size: 20px 20px;
				height: 100rpx;
				background-repeat: no-repeat;
				border-radius: 40rpx;
			}
		}
	}
	
</style>
