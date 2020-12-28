<template>
	<view class="body">
		<view :class="textColor">
			<text>{{num}}</text>
		</view>
		<view class="title-name">
			<text>{{titleName}}</text>
		</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				textColor: this.titleName === "重量偏差(t)" ? "yellow" : this.numColor
			}
		},
		props: {
			num:String,
			titleName:String,
			numColor: {
				type:String,
				default: "green"
			},
		},
	}
</script>

<style>
.body {
	background-color: white;
	display: flex;
	flex-direction: column;
}
.green {
	display: flex;
	justify-content: center;
	align-items: center;
	margin-top: 15rpx;
	font-size: 30rpx;
	background-color: #FFFFFF; 
	color: #00B589;
}

.yellow {
	display: flex;
	justify-content: center;
	align-items: center;
	margin-top: 15rpx;
	font-size: 30rpx;
	background-color: #FFFFFF; 
	color: #F7B400;
}

.black {
	display: flex;
	justify-content: center;
	align-items: center;
	margin-top: 15rpx;
	font-size: 30rpx;
	background-color: #FFFFFF;
	color: #666666;
}

.title-name {
	display: flex;
	justify-content: center;
	margin-top: 5rpx;
	font-size: 25rpx;
	background-color: #FFFFFF; 
	color: #666666;
	align-items: center;
}

</style>
