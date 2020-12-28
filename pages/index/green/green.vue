<template>
	<view class="body">
		<SectionView title="空气环境" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="56" titleName="扬尘达标天数" numColor="green"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="24" titleName="喷淋启用次数" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="34" titleName="喷淋用水(m3)" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="65" titleName="喷淋用电(kwh)" numColor="black"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="施工排水" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="8.1" titleName="PH值" numColor="green"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="14" titleName="浑浊度" numColor="green"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="3" titleName="异味" numColor="green"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="生活排水" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="5" titleName="PH值" numColor="green"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="3" titleName="浑浊度" numColor="green"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="3" titleName="异味" numColor="green"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="节地" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="222" titleName="覆盖和绿化(m2)" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="22.2" titleName="覆盖和绿化率(%)" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="中" titleName="覆盖绿化比" numColor="yellow"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="节材" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="234(吨)" titleName="混凝土" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="4(吨)" titleName="钢筋" numColor="black"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="节水" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="3.56" titleName="总市政用水(m3)" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="3.0" titleName="总回收用水(m3)" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="3.6" titleName="用水消耗" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="84.3" titleName="节水指数" numColor="yellow"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="节能" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="333" titleName="总用电(kwh)" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="1.5" titleName="用电消耗(kwh/万元)" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="136.6" titleName="节电指数" numColor="black"></AppNumTitleCell>
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
