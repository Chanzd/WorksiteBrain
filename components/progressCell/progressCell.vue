<template>
	<view class="body">
		<view class="left-text">
			<text style="font-size: 18rpx;">{{leftText}}</text>
		</view>
		<view class="progress">
			<u-line-progress active-color="#00BAF1" :percent="progress" ></u-line-progress>
		</view>
		<view class="right-text">
			<text style="font-size: 18rpx;">{{rightText}}</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {

			};
		},
		props: {
			leftText:String,
			progress:String,
			rightText:String
		}
	}
</script>

<style>
	.body {
		display: flex;
		flex-direction: row;
		background-color: white;
		padding: 15rpx;
	}
	.left-text .right-text {
		color: #666666;
		font-size: 12rpx;
	}
	.progress {
		margin-left: 30rpx;
		margin-right: 30rpx;
	}

</style>
