<template>
	<view class="noticeCenter-wrap">
		<view 
		:key="index"
		v-for="(item, index) in list"
		class="item pd30 dis_fl ju_sb">
			<view class="fs28 cl505050">
				{{item.text}}
			</view>
			<image class="arrow" src="../../static/img/common/common_icon_arrow.png" mode=""></image>
		</view>
	</view>
</template>

<script>
export default {
	data(){
		return{
			list:[
				{
					text: '关于上线现货平台量化交易A套餐的通知'
				},
				{
					text: '关于上线现货平台量化交易B套餐的通知'
				},
				{
					text: '关于上线现货平台量化交易'
				},
				{
					text: '现货平台量化交易A套餐'
				}
			]
		}
	},
	
};
</script>

<style lang="scss" scoped>
.noticeCenter-wrap {
	margin-top: 20upx;
	border-top:1px solid rgba(231,231,231,1);
	
	&>.item{
		background: #ffffff;
		border-bottom:1px solid rgba(231,231,231,1);
		&>.arrow{
			position: relative;
			top: 10upx;
			width: 30upx;
			height: 30upx;
		}
		
	}
}
</style>
