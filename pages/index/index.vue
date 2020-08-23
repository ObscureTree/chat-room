<template>
	<view class="content">
		<view class="top-bar">
			<view class="top-bar-left">
				<image src="../../static/f9Q5-imvgKpT1kSbw-az.jpg"></image>
			</view>
			<view class="top-bar-center">
				<image src="../../static/f9Q5-imvgKpT1kSbw-az.jpg" class="logo"></image>
			</view>
			<view class="top-bar-right">
				<view class="search">
					<image src="../../static/search@2x.png"></image>
				</view>
				<view class="add">
					<image src="../../static/add@2x.png"></image>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style lang="scss">
	.content {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	
	.top-bar {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		height:88rpx;
		box-sizing: border-box;
		background: $uni-bg-color;
		box-shadow: 0rpx 1rpx 0rpx 0rpx $uni-border-color;
		padding-left: $uni-spacing-col-base;
		padding-right: $uni-spacing-col-base;
		
		.top-bar-left {
			float: left;
			image {
				margin-top: 10rpx;
				width: 68rpx;
				height: 68rpx;
				border-radius: 16rpx;
			}
		}
		
		.top-bar-center {
			position: absolute;
			text-align: center;
			left: 0;
			right: 0;
			top: 0;
			bottom: 0;
			//border: 1rpx solid red;
			margin: auto;
			.logo {
				padding-top: 19rpx;
				width: 88rpx;
				height: 42rpx;
			}
		}
		
		.top-bar-right {
			float: right;
			.search {
				width: 88rpx;
				height: 88rpx;
				display: inline-block;
				//border: 1px solid red;
			}
			.add {
				width: 88rpx;
				height: 88rpx;
				display: inline-block;
				//border: 1px solid red
			}
			image {
				padding: 18rpx 0 0 18rpx;
				width: 52rpx;
				height: 52rpx;
			}
		}
	}

</style>
