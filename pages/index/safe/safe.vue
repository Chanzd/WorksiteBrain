<template>
	<view class="body">
		<SectionView title="安全教育" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="976" titleName="wifi在线累计" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="345" titleName="进场教育累计" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="456" titleName="三级教育累计" numColor="black"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="安全交底" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="433" titleName="今日新增次数" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="124" titleName="本月新增次数" numColor="black"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="今日巡更" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="4" titleName="定点巡更" numColor="green"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="1" titleName="线路巡更" numColor="green"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="0" titleName="异常点" numColor="green"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="安全检查" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="0" titleName="今日新增" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="13" titleName="累计待整改" numColor="yellow"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="59.4%" titleName="累计完成率" numColor="green"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="安全管理" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="123" titleName="危险源累计分布" numColor="yellow"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="444" titleName="应急演练次数" numColor="green"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="设备监控" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="0" titleName="报警" numColor="yellow"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="0" titleName="违章" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="0" titleName="提醒" numColor="black"></AppNumTitleCell>
		</view>
		<view class="line-view">
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
	.AppCard {
		display: flex;
		flex-direction: row;
		padding: 30rpx;
	}
	.cell {
		flex-grow: 1;
	}
	.line-view {
		background-color: #EDEDED;
		height: 20rpx;
	}

</style>
