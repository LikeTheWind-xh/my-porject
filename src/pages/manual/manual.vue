<template>
	<view>
<<<<<<< HEAD
		<nav-head title="手动收纸"></nav-head>
=======
		<view class="nav">
			<u-icon name="arrow-left" @click="rollback"></u-icon>
			<text>手动收纸</text>
		</view>
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
		<view class="head">
			<image src="../../static/manual/background.png"></image>
		</view>
		<view class="aircraft">
			<image src="../../static/manual/aircraft.png"></image>
		</view>
		<view class="title">
			<text>环保健康又获利</text>
		</view>
		<view class="form">
			<view class="form-title">
				<text style="font-weight: 900;color: #18B566;margin-right:10px">|</text>
				<text style="font-weight: 700;"> 手动收报</text>
			</view>
			<view class="item">
				<text class="item-title">联系人</text>
				<u-input placeholder="请输入联系人名称" />
			</view>
			<view class="item">
				<text class="item-title">手机号</text>
				<u-input placeholder="请输入联系号码" />
			</view>
			<view class="item">
				<text class="item-title">地址</text>
				<u-input placeholder="武大航域2区A2栋" />
			</view>
				<view class="postscript">
					<text class="postscript-title">备注</text>
					<view class="input">
						<u-input type="textarea" height=150 :placeholder="content"  />
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
				content:"多行输入"
			};
		},
		methods:{
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
	.form text{
		font-size: 26rpx;
	}
<<<<<<< HEAD

=======
	.nav {
		// position: absolute;
		margin-top: 25rpx;
		width: 100%;
		height: 100rpx;

		display: flex;
		align-items: center;

		text {
			font-size: 25rpx;
			font-weight: 600;
			margin-left: 20rpx;
			// color: white;
		}
	}
>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9

	.head {
		width: 100%;
		height: 30vh;
<<<<<<< HEAD
		margin-top: -120rpx;
=======
		margin-top: -80rpx;

>>>>>>> 2505fc121ea30ac735dc49bb59d83ee1215ab6f9
		image {
			width: 100%;
			height: 100%;
		}
		z-index: -1;
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
		}

		.postscript{
			text{
				margin-left: 15%;
				
			}
		}

		.item {
			display: flex;
			justify-content: space-around;
			align-items: center;
			width: 90%;
			padding-left: 10rpx;
			margin: 0 auto;
			margin-top: 40rpx;
			border-radius: 20rpx;
			box-shadow: 5px 5px 25px 5px rgb(228, 245, 237);
			margin-bottom: 20rpx;
		}
	}
	.input{
		// width: 750rpx;
		width: 90%;
		// margin-left: 8%;
		padding-left: 60rpx;
		margin: 0 auto;
		margin-top: 20rpx;
		border-radius: 20rpx;
		box-shadow: 5px 5px 25px 5px rgb(228, 245, 237);
	}
</style>
