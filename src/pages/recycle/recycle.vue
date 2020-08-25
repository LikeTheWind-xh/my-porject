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
		<view class="num">
			<view></view>
			<text>您已累计拯救{{num}}棵小树</text>
		</view>

		<view class="content">
			<vite class="title">
				<text>回收记录</text>
			</vite>
			<view class="time">
				<text class="timeTitle">时间</text>
				<view v-for="item in number" :key="item">
					<image src="../../static/common/icon.png"></image>
					<text class="leftDate">2020-10-10</text>
					<text class="rightDate">10:00</text>
				</view>
			</view>
		</view>

		<view class="waiter">
			<text>客服/投诉电话:18564713251</text>
		</view>

		<view class="home_me">
			<view class="home">
				<button style="background-image: url(../../static/common/home.png);"></button>
				<text>首页</text>
			</view>
			<view class="me">
<<<<<<< HEAD
				<button style="background-image: url(../../static/common/me.png);background-color:#53DC9C;"></button>
=======
				<button  style="background-image: url(../../static/common/me.png);background-color:#53DC9C;"></button>
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
				<text>我的</text>
			</view>
		</view>
	</view>
</template>

<script>
<<<<<<< HEAD
	import navHead from "../../components/nav/nav-head.vue"
	export default {
		components:{
			navHead
		},
=======
	

	export default {
	
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
		data() {
			return {
				num: 10,
				number: [1, 2, 3]
			}
		},
		methods: {

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

	.num {
		width: 90%;
		height: 60rpx;
		margin: 0 auto;
		margin-top: 20rpx;
		border-radius: 50rpx;
		color: white;
		display: flex;
		align-items: center;
		background-image: linear-gradient(to right, #28CD80 0%, #94F3C7 100%);

		view {
			margin-left: 40rpx;
			width: 10rpx;
			height: 60%;
			border-radius: 50rpx;
			background-color: white;
		}

		text {
			margin-left: 20rpx;
		}
	}

	.content {
		width: 90%;
		// height: 500rpx;
		margin: 0 auto;
		margin-top: 30rpx;
		box-shadow: 1px 1px 1px 1px #DCDFE6;
		border-radius: 50rpx;
		display: flex;
		flex-direction: column;
		padding-left: 5%;

		.title {
			margin-top: 40rpx;
			font-size: 28rpx;
			font-weight: 700;
			margin-bottom: 20rpx;
		}

		.time {
			.timeTitle {

				font-size: 28rpx;
				// font-weight: ;
			}

			view {
				display: flex;

				.leftDate {
					margin-left: 5%;
					font-size: 28rpx;
					font-weight: 800;
				}

				.rightDate {
					margin-left: 40%;
					color: #989898;
				}

				margin-top: 6%;
				margin-bottom: 4%;
			}

			image {
				width: 40rpx;
				height: 40rpx;
			}
		}
	}

	.waiter {
		width: 100%;
		position: absolute;
		text-align: center;
		bottom: 15%;
		// line-height: 100rpx;
		color: #989898;
	}

<<<<<<< HEAD
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
=======
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
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
</style>
