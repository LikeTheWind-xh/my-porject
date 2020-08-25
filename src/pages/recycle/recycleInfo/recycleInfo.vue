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
		<view class="info">
			<view class="DateTitle">
				
				<view>
					<text>2020-08-03 10:00:00</text>
					<button>回收详情</button>
				</view>
			</view>

			<view class="recycleInfo">
				<view>
					<text class="title">地址</text>
					<text class="content">万科城花上东10区202</text>
				</view>
				<view>
					<text class="title">联系人</text>
					<text class="content">宇宙男神</text>
				</view>
				<view>
					<text class="title">联系电话</text>
					<text class="content">18456354788</text>
				</view>
				<view style="border-bottom: 1rpx solid #F1F1F1;height: 200rpx">
					<text class="title">店铺门头照</text>
					<image class="content" style="width:300rpx;height: 150rpx;" mode="aspectFill" src="../../../static/activa/logo.png"></image>
				</view>
				<view>
					<text class="title">备注</text>
					<text class="content">多放香菜,少放辣</text>
				</view>
			</view>


		</view>
		<view class="map">
			<map style="width: 100%;height: 100%;border-radius: 50rpx;">

			</map>
		</view>

		<view class="foot">
			<button @click="back">返回</button>
			<button>已上门</button>
		</view>
	</view>
</template>

<script>
	import navHead from "../../../components/nav/nav-head.vue"
	export default {
		components:{
			navHead
		},
		data() {
			return {

			}
		},
		methods: {
<<<<<<< HEAD
=======
			rollback(){
				uni.navigateBack({
					delta:1
				})
			}
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
		}
	}
</script>

<style lang="scss">
	page {
		background-color: #F5F5F5;
	}
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
	.info {
		width: 95%;
		border-radius: 50rpx;
		/* border: 1rpx solid white; */
		margin: 0 auto;
		background-color: white;
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.DateTitle {

		width: 100%;
		view{
			width: 90%;
			margin: 0 auto;
			display: flex;
			justify-content: space-between;
			flex-wrap: nowrap;
			button {
				width: 27%;
				height: 50rpx;
				background-color: #28CD80;
				color: white;
				border-radius: 50rpx;
				line-height: 50rpx;
				font-size: 24rpx;
				margin-left: 25%;
				
			}
			
			text {
				width: 55%;
				font-weight: 900;
			}
			
			margin: 0 auto;
			margin-top: 3%;
			margin-bottom: 2%;
		}
		border-bottom: 1rpx solid #F1F1F1;
	}



	.map {
		width: 90%;
		margin: 0 auto;
		height: 350rpx;
		margin-top: 40rpx;
		border-radius: 50rpx;
		background-color: white;
	}

	.foot {
		display: flex;
		justify-content: center;

		button {
			width: 180rpx;
			height: 70rpx;
			border-radius: 50rpx;
			line-height: 70rpx;
			color: white;
			background-color: #28CD80;
			margin-top: 80rpx;
			
		}
	}

	.recycleInfo {
		width: 90%;
		margin-top: 30rpx;

		view {
			display: flex;
			// justify-content: space-between;
			margin-top: 20rpx;
			margin-bottom: 20rpx;

			.title {
				font-size: 28rpx;
				// font-weight: 700;

			}

			text:nth-child(1) {
				color: #B3B3B3;
			}

			text:nth-child(2) {
				font-weight: 600;
				color: #000000;
			}

			.content {
				position: absolute;
				left: 40%;
			}

		}
	}
</style>
