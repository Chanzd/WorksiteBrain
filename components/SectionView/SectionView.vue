<template>
	<view class="body">
		<view class="section-view">
			<view :class="bgColor">
			</view>
			<view class="title-name">
				{{title}}
			</view>
		</view>
		<u-line class="line" color="#DDDDDD"></u-line>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				bgColor: this.color === "blue" ? "blue":"green"
			};
		},
		props:{
			title:String,
			color:String
		}
	}
</script>

<style>
	.body {
		display: flex;
		flex-direction: column;
		background-color: white;
		height: 80rpx;
		padding: 20rpx;
	}
	.section-view {
		display: flex;
		flex-direction: row;
		align-items: center;
		height: 78rpx;
	}
	.blue {
		width: 5rpx;
		height: 20rpx;
		background-color: #2B85E4;
	}
	.green {
		width: 5rpx;
		height: 20rpx;
		background-color: #00b589;
	}
	.title-name {
		font-size: 16rpx;
		color: #666666;
		margin-left: 10rpx;
	}
	.line {
		margin-left: 15rpx;
		margin-right: 15rpx;
	}
	
</style>
