<template>
	<view>
<<<<<<< HEAD
		<nav-head title="店铺码激活"></nav-head>
=======
		<view class="nav">
			<u-icon name="arrow-left" @click="rollback"></u-icon>
			<text>店铺码激活</text>
		</view>
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
		<view class="head">

			<image src="../../static/manual/background.png"></image>
		</view>
		<view class="aircraft">
			<image src="../../static/activa/logo.png"></image>
		</view>
		<view class="title">
			<text>轻松4步即可激活</text>
		</view>
		
		<view class="form">
			<view class="form-title">
				<text style="font-weight: 900;color: #18B566;margin-right:10px">|</text>
				<text style="font-weight: 700;"> 店铺码激活</text>
			</view>
			<view class="item">
				<text class="item-title">名称</text>
				<u-input placeholder="输入店铺名字" />
			</view>
			<view class="item">
				<text class="item-title">手机号</text>
				<u-input placeholder="输入联系号码" />
			</view>
			<view class="item">
				<text class="item-title">地址</text>
				<u-input placeholder="武大航域2区A2栋" />
			</view>
			<view class="file">
				<text class="file">店铺门头照片</text>
				<view class="uploadFile">
					<button style="font-size:20px">+</button>
				</view>
			</view>
		</view>

		<u-button shape="circle" type="success" style="width: 80%;position: absolute;bottom: 10%;left:10%;">点击确定</u-button>

	</view>
</template>

<script>
	import navHead from "../../components/nav/nav-head.vue"
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
	.uni-button:after {
		content: ""
	}
<<<<<<< HEAD

	.head {
		width: 100%;
		height: 30vh;
		margin-top: -120rpx;
=======
	.nav{
		// position: absolute;
		margin-top: 20rpx;
		width: 100%;
		height: 100rpx;
	
		display: flex;
		align-items: center;
		text{
			font-size: 30rpx;
			font-weight: 700;
			margin-left: 20rpx;
			// color: white;
		}
	}
	.head {
		width: 100%;
		height: 30vh;
		margin-top: -80rpx;
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
		image {
			width: 100%;
			height: 100%;
		}
	}

	.title {
		width: 80%;
		position: absolute;
		z-index: 10;
<<<<<<< HEAD
		top: 15%;
		left: 13%;
=======
		top: 18%;
		left: 10%;
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
		height: 80rpx;
		font-size: 35rpx;
		letter-spacing: 5rpx;
		color: white;
		margin: 0 auto;
	}

	.aircraft {
		width: 200rpx;
		height: 200rpx;
		position: absolute;
<<<<<<< HEAD
		top: 160rpx;
=======
		top: 180rpx;
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
		z-index: 1;
		image {
			width: 100%;
			height: 100%;
		}

		margin-left: 60%;
	}

	.form {
		width: 90%;
		margin: 0 auto;
		background-color: #FFFFFF;
		// margin-top: -100rpx;
		position: absolute;
		top: 23%;
		left: 5%;
		border-radius: 20rpx;
		border: 5rpx solid white;
		.form-title {
			width: 90%;
			margin: 0 auto;
			margin-top: 50rpx;
			margin-bottom: 50rpx;
			font-weight: 700;
		}
		.file{
			width: 90%;
			margin-top: 2%;
<<<<<<< HEAD
=======
			margin-left: 55rpx;
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
			display: flex;
			flex-direction: column;
			text{
				margin-bottom: 20rpx;
			}
<<<<<<< HEAD
			margin: 0 auto;
=======
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
		}
		.item {
			display: flex;
			justify-content: space-around;
			align-items: center;
			width: 90%;
			padding-left: 20rpx;
			margin: 0 auto;
			margin-top: 40rpx;
			border-radius: 20rpx;
			box-shadow: 5px 5px 25px 5px rgb(228, 245, 237);

		}
	}

	.uploadFile {
		background-color: #F1F2F6;
		width: 100%;
		height: 15vh;
		display: flex;
		align-items: center;
		border: none;
		border-radius: 20rpx;
		margin-bottom: 20rpx;
		button {
			width: 100rpx;
			height: 100rpx;
			background-color: white;
			border-radius: 50%;
		}

	}

	uni-button:after {
		content: "" !important;
		border: none !important;
	}
</style>
