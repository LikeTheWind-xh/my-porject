<template>
	<view class="main">
		<image src="../../static/login/background.png" class="backgroundImage" mode=""></image>
		<view class="content">
			<view class="title">
				<text>欢迎来到接废纸啰</text>
			</view>
			<view class="login">

				<view class="item">
					<image src="../../static/login/email.png"></image>
					<input type="text" placeholder="请输入账号" class="input" />
				</view>
				<view class="item">
					<image src="../../static/login/pwd.png"></image>
					<input :type="type" placeholder="请输入密码" class="input" />
					<image v-if="!isShow" src="../../static/login/eye.png" @click="Show" class="eye"></image>
					<image v-else src="../../static/login/visible.png" class="eye" @click="Show"></image>
				</view>

				<view class="register_repwd">
					<text>注册></text>
					<text>忘记密码</text>
				</view>

				<button class="submit">登录</button>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				isShow: false,
				type: "password"
			}
		},
		methods: {
			Show() {
				this.isShow = !this.isShow
				if (this.isShow)
					this.type = "text"
				else
					this.type = "password"
			}
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
	.title{
		text{
			font-size: 40rpx;
			font-weight: 700;
		}
	}
	.main {
		width: 100%;
		height: 100vh;
		margin: 0 auto;
	}

	.content {
		width: 90%;
		margin: 0 auto;
		margin-top: 30%;
		height: 50%;

	}

	.login {
		margin-top: 20%;
	}

	.item {
		display: flex;
		border-bottom: 1rpx solid #F1F1F1;
		margin-top: 80rpx;
		image {
			width: 40rpx;
			height: 40rpx;
			padding-left: 20rpx;
			margin-bottom: 20rpx;
		}
		.eye {
			width: 40rpx;
			height: 28rpx;
			margin-left: 25%;
		}

		.input {
		
			margin-left: 50rpx;
		}
	}

	.register_repwd {
		display: flex;
		justify-content: space-between;
		margin-top: 50rpx;
		color: #B5B5B5;
		margin-bottom: 200rpx;
		font-size: 30rpx;
	}
	
	.submit{
		width: 80%;
		border-radius: 50rpx;
		background-color: #28CD80;
		color: white;
	}
</style>
