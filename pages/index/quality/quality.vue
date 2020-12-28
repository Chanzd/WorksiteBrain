<template>
	<view class="body">
		<SectionView title="创优工坊" color="green"></SectionView>
		<view class="video">
			<video id="myVideo" src="https://img.cdn.aliyun.dcloud.net.cn/guide/uniapp/%E7%AC%AC1%E8%AE%B2%EF%BC%88uni-app%E4%BA%A7%E5%93%81%E4%BB%8B%E7%BB%8D%EF%BC%89-%20DCloud%E5%AE%98%E6%96%B9%E8%A7%86%E9%A2%91%E6%95%99%E7%A8%8B@20200317.mp4"></video>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="质量检查" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="23" titleName="今日新增" numColor="yellow"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="6" titleName="今日完成整改" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="55%" titleName="累计完成率(%)" numColor="black"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="质量文件(份)" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="376" titleName="质保资料" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="165" titleName="实体检测" numColor="black"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="质量动态" color="green"></SectionView>
		<view class="list-cell">
			<view class="image">
				<u-image width="100rpx" height="65rpx" src="/static/1.jpg"></u-image>
			</view>
			<view class="text-container">
				<view class="text">非基督教徒安静地</view>
				<view class="text">2019-04-10</view>
			</view>
		</view>
	</view>
</template>

<script>
	import SectionView from "@/components/SectionView/SectionView.vue"
	import AppNumTitleCell from "@/components/AppCardCell/AppNumTitleCell/AppNumTitleCell.vue"
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		},
		components: {
			SectionView,
			AppNumTitleCell
		}
	}
</script>

<style>
	.body {
		display: flex;
		flex-direction: column;
	}
	.video {
		padding: 15rpx;
	}
	
	.line-view {
		background-color: #EEEEEE;
		height: 20rpx;
	}
	.AppCard {
		display: flex;
		flex-direction: row;
		padding: 30rpx;
	}
	.cell {
		flex-grow: 1;
	}
	
	.list-cell {
		display: flex;
		flex-direction: row;
		height: 100rpx;
		padding-left: 30rpx;
	}
	.image {
		width: 100rpx;
		height: 65rpx;
	}
	.text-container {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		padding-left: 15rpx;
		height: 70rpx;
	}
	.text {
		font-size: 16rpx;
		color: #666666;
	}

</style>
