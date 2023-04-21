<template>
	<view class="top">
		<swiper class="swiper" circular :indicator-dots="indicatorDots" :autoplay="autoplay" :interval="interval"
			:duration="duration">
			<swiper-item>
				<view class="swiper-item uni-bg-red">
					<image src="@/static/banner.png" mode=""></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item uni-bg-green">
					<image src="@/static/goods3.jpg" mode=""></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item uni-bg-blue">
					<image src="@/static/goods2.jpg" mode=""></image>
				</view>
			</swiper-item>
			<swiper-item>
				<view class="swiper-item uni-bg-blue">
					<image src="@/static/goods1.jpg" mode=""></image>
				</view>
			</swiper-item>
		</swiper>
		<view class="search">
			<input type="text" placeholder="搜美食,菜谱">
			<image class="search" src="@/static/3.png" mode=""></image>
		</view>

		<view class="nav">
			<view class="nav_every">
				<image src="@/static/5.png" mode=""></image>
				<text>餐宴</text>
			</view>
			<view class="nav_every">
				<image src="@/static/7.png" mode=""></image>
				<text>餐宴</text>
			</view>
			<view class="nav_every">
				<image src="@/static/4.png" mode=""></image>
				<text>餐宴</text>
			</view>
			<view class="nav_every">
				<image src="@/static/6.png" mode=""></image>
				<text>餐宴</text>
			</view>
		</view>
		<view class="banner">
			<image src="@/static/8.png" mode=""></image>
		</view>
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
			}
		}
	}
</script>

<style lang="scss">
	body {
		background-color: #eeeeee;
	}

	.top {
		width: 100%;
		background-color: white;

		.swiper {
			height: 460rpx;

			swiper-item {
				image {
					width: 100%;
				}
			}
		}



		.search {
			margin: 0 auto;
			width: 94%;
			height: 130rpx;

			input {
				padding-left: 35%;
				box-sizing: border-box;
				border: 1px solid black;
				background-color: white;

			}
		}

		.nav {
			display: flex;
			width: 94%;
			margin: 60rpx auto;

			.nav_every {
				width: 25%;
				text-align: center;

				image {
					width: 150rpx;
					height: 150rpx;
				}
			}
		}

		.banner {
			image {
				width: 100%;
				margin-bottom: 30rpx;
			}
		}
	}
</style>