<template>
	<view class="content">
		<u-image width="100%" height="225rpx" src="/static/1.jpg"></u-image>
		<view class="text-area">
			<text class="title">{{title}}</text>
		</view>
		<view class="app-view">
			<view class="apps" v-for="item in AppArr" :key="item.title">
			    <view class="click icon" @click="clickIcon(item.title)">
					<view class="image-icon">
						<u-image
						  width="50rpx"
						  height="50rpx"
						  :src="`/static/${item.icon}.png`">
						</u-image>
					</view>
					<text>{{item.title}}</text>
				</view>
			</view>
		</view>
		<view class="view-bg">
			<view class="card-container" v-for="item in CardArr" :key="item.title">
				<view class="AppCard">
					<AppCardCell :title="item.title" :icon="item.icon" :titleArr="item.titleArr" :numArr="item.numArr"></AppCardCell>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	import AppCardCell from "@/components/AppCardCell/AppCardCell.vue"
	export default {
		data() {
			return {
				title: '上海浦东芜湖小区项目',
				AppArr: [
					{icon:"progress",title:"进度"},
					{icon:"safe",title:"安全"},
					{icon:"quality",title:"质量"},
					{icon:"operate",title:"经营"},
					{icon:"greenConstruct",title:"绿色施工"}
				],
				CardArr: [
					{title:"今日出勤",icon:"attendance",titleArr:["实时在场(人)","累计进场(人)","出勤率"],numArr:["0","0","0%"]},
					{title:"设备功效",icon:"equipment",titleArr:["在线设备","累计吊次","累计吊重(t)"],numArr:["0","0","0"]},
					{title:"砼消耗",icon:"concrete",titleArr:["料单总量(t)","称重总量(t)","重量偏差(t)"],numArr:["0","0","0"]},
					{title:"今日检查",icon:"check",titleArr:["新增(项)","完成整改(项)","新增安全事项(项)"],numArr:["0","0","0"]},
					{title:"现场环境",icon:"environment",titleArr:["6˚C～13˚C","TSP实测(µg/m³)","废水PH值"],numArr:["多云","-","8.1"]}
				]
			}
		},
		onLoad() {
			
		},
		methods: {
			clickIcon: function (str) {
				
				if (str == '进度') {
					uni.navigateTo({
						url:'progress/progress'
					})
				} else if (str === '安全') {
					uni.navigateTo({
						url:'safe/safe'
					})
				} else if (str === '质量') {
					uni.navigateTo({
						url:'quality/quality'
					})
				} else if (str === '经营') {
					uni.navigateTo({
						url:'operate/operate'
					})
				} else if (str === '绿色施工') {
					uni.navigateTo({
						url:'green/green'
					})
				}
				console.log(str);
			}
		},
		components:{
			AppCardCell
		}
	}
</script>

<style>
	.content {
		display: flex;
		flex-direction: column;
		background-color: #F7F7F7;
		height: 1600rpx;
	}

	.text-area {
		position: absolute;
		top: 150rpx;
		left: 15rpx;
		height: 16;
	}

	.title {
		font-size: 16rpx;
		color: #FFFFFF;
	}
	
	.app-view {
		padding: 20rpx;
		margin-top: 20rpx;
		margin-left: 15rpx;
		margin-right: 15rpx;
		display: flex;
		flex-wrap: wrap;
		background-color: #FFFFFF;
		border-radius: 5rpx;
	}
	
	.apps {
		text-align: center;
		width: 20%;
		margin-bottom: 15rpx;
	}
	
	.image-icon {
		position: relative;
		width: 50rpx;
		height: 50rpx;
		margin: 0 auto 8rpx;
		border-radius: 10rpx;
	}
	
	.card-container {
		flex-direction: column;
		justify-content: space-between;
		background-color: #F7F7F7;
		margin-top: 20rpx;
		padding: 10rpx;
	}
	
	.AppCard {
		min-height: 200rpx;
		border-radius: 10rpx;
		background-color: white;
		flex: 1;
	}
	
</style>
