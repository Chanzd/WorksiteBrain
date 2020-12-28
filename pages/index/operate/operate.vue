<template>
	<view class="body">
		<SectionView title="经营分析(万元)" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="50.0" titleName="累计报量" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="1000.0" titleName="审批金额" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="150.0" titleName="实付金额" numColor="green"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="150.0" titleName="未付金额" numColor="yellow"></AppNumTitleCell>
		</view>
		<view class="line-view">
		</view>
		<SectionView title="工程索赔" color="green"></SectionView>
		<view class="AppCard">
			<AppNumTitleCell class="cell" num="223" titleName="获签日期(份)" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="123" titleName="获签费用(万)" numColor="black"></AppNumTitleCell>
			<AppNumTitleCell class="cell" num="56" titleName="反索赔(份)" numColor="green"></AppNumTitleCell>
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
