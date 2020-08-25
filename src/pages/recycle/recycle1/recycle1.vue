<template>
	<view class="main">
<<<<<<< HEAD
		<nav-head title="回收记录"></nav-head>
=======
		<view class="nav">
			<u-icon name="arrow-left" @click="rollback"></u-icon>
			<text>回收记录</text>
		</view>
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
		<view class="circle">
			<button>回收次数</button>
			<text>共<text style="font-size: 80rpx;font-weight: 800;">10</text>次</text>
		</view>

		<view class="title">
			<text class="title">回收记录</text>
		</view>

		<view class="time">
			<view class="info" v-for="item in num" :key="item" @click="skip">
				<image src="../../../static/common/icon.png"></image>
				<text class="leftDate"> &nbsp; &nbsp;2020-10-10</text>
				<text class="rightDate">10:00:00</text>
				<text class="addrs">万科城花圆</text>
				<text style="font-weight: 800;">></text>
			</view>
		</view>
		<view class="home_me">
			<view class="home">
				<button style="background-image: url(../../../static/common/home.png);"></button>
				<text>首页</text>
			</view>
			<view class="me">
				<button  style="background-image: url(../../../static/common/me.png);background-color:#53DC9C;"></button>
				<text>我的</text>
			</view>
		</view>
	</view>
</template>

<script>
<<<<<<< HEAD
	import navHead from "../../../components/nav/nav-head.vue"
	export default {
		components:{
			navHead
		},
=======

	export default {
		
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
		data() {
			return {
				num: [1, 2, 3]
			}
		},
		methods: {
			skip(){
				uni.navigateTo({
					url:"../recycleInfo/recycleInfo"
				})
			}
		}
	}
</script>

<style lang="scss">
	.nav{
		height: 180rpx;
		display: flex;
		align-items: center;
		text {
			font-size: 30rpx;
			font-weight: 700;
			margin-left: 20rpx;
		}
	}
	.circle {
		width: 200px;
		height: 200px;
		background: #ffffff;
		border-radius: 50%;
		border: 20px solid #D3F2E4;
		margin: 0 auto;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;

		button {
			width: 70%;
			height: 50rpx;
			// margin-top: 30%;
			background-color: #28CD80;
			color: white;
			// margin: 0 auto;
			border-radius: 50rpx;
			line-height: 50rpx;

		}

		text {
			margin-top: 50rpx;
			font-size: 40rpx;
			color: #28CD80;
		}
	}

	.title {
		width: 90%;
		margin: 0 auto;
		font-size: 28rpx;
		font-weight: 800;
		margin-top: 15%;
	}

	.time {
		width: 90%;
		margin: 0 auto;
		margin-top: 30rpx;
		box-shadow: 1px 1px 1px 1px #DCDFE6;
		border-radius: 50rpx;
		padding-left: 3%;
		display: flex;
		flex-direction: column;

		.info {
			width: 90%;
			display: flex;
			border: 1rpx solid white;
			border-radius: 50rpx;
			background-color: #FBFBFB;
			margin-top: 20rpx;
			margin-bottom: 20rpx;

			image {
				width: 40rpx;
				height: 40rpx;
			}

			.leftDate {
				// margin-left: 5%;
				font-size: 28rpx;
				font-weight: 800;
			}

			.rightDate {
				// margin-left: 30%;
				color: #989898;
			}

			.addrs {
				width: 20%;
				margin-left: 24%;
				overflow: hidden;
				white-space: nowrap;
				text-overflow: ellipsis;
			}

		}

	}

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
			background-color: #D4D4D4;
			background-repeat: no-repeat;
			border-radius: 40%;
		}
	}
}
</style>
