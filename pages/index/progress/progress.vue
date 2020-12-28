<template>
	<view class="body">
		<SectionView title="形象进度" color="blue"></SectionView>
		<progressCell leftText="工程进度" progress="100" rightText="16(天)"></progressCell>
		<progressCell leftText="产值进度" progress="0" rightText="5.00(亿元)"></progressCell>
		<progressCell leftText="工程款进度" progress="0" rightText="5.00(亿元)"></progressCell>
		<view class="line-view">
		</view>
		<SectionView title="浮光掠影" color="blue"></SectionView>
			<view class="video">
				<video id="myVideo" src="https://img.cdn.aliyun.dcloud.net.cn/guide/uniapp/%E7%AC%AC1%E8%AE%B2%EF%BC%88uni-app%E4%BA%A7%E5%93%81%E4%BB%8B%E7%BB%8D%EF%BC%89-%20DCloud%E5%AE%98%E6%96%B9%E8%A7%86%E9%A2%91%E6%95%99%E7%A8%8B@20200317.mp4"></video>
			</view>
		<view class="line-view">
		</view>
		<SectionView title="BIM进度模拟" color="blue"></SectionView>
		<view class="video">
			<video id="myVideo" src="https://img.cdn.aliyun.dcloud.net.cn/guide/uniapp/%E7%AC%AC1%E8%AE%B2%EF%BC%88uni-app%E4%BA%A7%E5%93%81%E4%BB%8B%E7%BB%8D%EF%BC%89-%20DCloud%E5%AE%98%E6%96%B9%E8%A7%86%E9%A2%91%E6%95%99%E7%A8%8B@20200317.mp4"></video>
		</view>
		<view class="line-view">
		</view>
	</view>
</template>

<script>
	import SectionView from "@/components/SectionView/SectionView.vue"
	import progressCell from "@/components/progressCell/progressCell.vue"
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			
		},
		components:{
			SectionView,
			progressCell
		}
	}
</script>

<style>
	.body {
		display: flex;
		flex-direction: column;
	}
	.line-view {
		background-color: #EEEEEE;
		height: 20rpx;
	}
	.video {
		padding: 15rpx;
	}
	#myVideo {
		
	}

</style>
