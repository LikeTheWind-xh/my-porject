<template>

	<view class="nav">
		<u-icon name="arrow-left" @click="rollback"></u-icon>
		<text>{{title}}</text>
	</view>

</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			rollback(){
				uni.navigateBack({
					delta:1
				})
			}
		},
		props:{
			title:String
		}
	}
</script>

<style lang="scss">
	.nav {
		height: 180rpx;
		display: flex;
		align-items: center;

		text {
			font-size: 30rpx;
			font-weight: 700;
			margin-left: 20rpx;
		}
	}
</style>
