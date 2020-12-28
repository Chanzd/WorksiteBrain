<template>
	<view class="body">
		<view class="view-icon">
			<view class="image">
				<u-image
				  width="40rpx"
				  height="40rpx"
				  :src="`/static/${iconImg}.png`">
				</u-image>
			</view>
			<view class="title">
				{{iconTitle}}
			</view>
		</view>
		<view class="num-view">
			<AppNumTitleCell class="cell" :num="numArr[0]" :titleName="titleArr[0]"></AppNumTitleCell>
			<AppNumTitleCell class="cell" :num="numArr[1]" :titleName="titleArr[1]"></AppNumTitleCell>
			<AppNumTitleCell class="cell" :num="numArr[2]" :titleName="titleArr[2]"></AppNumTitleCell>
		</view>
	</view>
</template>

<script>
	import AppNumTitleCell from "@/components/AppCardCell/AppNumTitleCell/AppNumTitleCell.vue"
	export default {
		data() {
			return {
				iconTitle:this.title,
				iconImg:this.icon
			};
		},
		props:{
			type: String,
			title: String,
			icon:String,
			titleArr:Array,
			numArr:Array
		},
		methods:{
			
		},
		components:{
			AppNumTitleCell
		}
	}
</script>

<style>
	.body {
		display: flex;
		flex-direction: column;
		flex-wrap: wrap;
		background-color: white;
		padding: 15rpx;
	}
	
	.view-icon {
		display: flex;
		flex-direction: row;
	}
	
	.title {
		font-size: 20rpx;
		background-color: #1acd78; 
		color: white;
		margin-left: 10rpx;
		transform:matrix(1,0,-0.2,1,0,0);
		padding-left: 5rpx;
		padding-right: 5rpx;
	}
	.num-view {
		display: flex;
		flex-direction: row;
	}
	.cell {
		flex-grow: 1;
	}
	
</style>
