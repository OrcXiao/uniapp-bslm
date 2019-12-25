<template>
	<view class="pd30 home-wrap">
		<!-- start head -->
		<view class="dis_fl head">
			<image class="user-icon" src="../../static/img/home/home_navbar_avater.png" mode="scaleToFill"></image>
			<view class="cl505050 fs26 advert-wrap">
				<image class="advert-icon" src="../../static/img/home/home_navbar_icon_notice.png" mode="scaleToFill"></image>
				平台开放现货量化交易A套餐
			</view>
			<image class="info-icon" src="../../static/img/home/home_navbar_icon_notice_center.png" mode="scaleToFill"></image>
		</view>
		<!-- end head -->
		<!-- start swiper -->
		<view class="swiper-wrap">
			<swiper class="swiper" :indicator-dots="indicatorDots" :autoplay="autoplay" :interval="interval" :duration="duration">
				<swiper-item>
					<image class="user-icon" src="../../static/img/home/home_banner_one.png" mode="scaleToFill"></image>
				</swiper-item>
				<swiper-item>
					<image class="user-icon" src="../../static/img/home/home_banner_two.png" mode="scaleToFill"></image>
				</swiper-item>
				<swiper-item>
					<image class="user-icon" src="../../static/img/home/home_banner_therr.png" mode="scaleToFill"></image>
				</swiper-item>
			</swiper>
		</view>
		<!-- end head -->
	</view>
</template>

<script>
export default {
	data() {
		return {
			indicatorDots: true,
			autoplay: true,
			interval: 2000,
			duration: 500
		};
	},
	onLoad() {},
	methods: {}
};
</script>

<style lang="scss" scoped>
.home-wrap {
	padding-top: var(--status-bar-height);
	& > .head {
		& > .user-icon {
			width: 64upx;
			height: 64upx;
		}
		& > .advert-wrap {
			margin: 0 30upx;
			width: 515upx;
			height: 60upx;
			line-height: 60upx;
			background: #f1f1f1;
			border-radius: 30upx;

			& > .advert-icon {
				position: relative;
				top: 10upx;
				margin: 0 20upx;
				width: 36upx;
				height: 36upx;
			}
		}

		& > .info-icon {
			width: 42upx;
			height: 42upx;
			position: relative;
			top: 10upx;
		}
	}
	& > .swiper-wrap {
	}
}
</style>
