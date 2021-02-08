<template>
	<view class="container">

		<!-- 顶部 -->
		<view class="header">
			<view class="logo">
				<image src="../../static/images/logo.png" mode=""></image>
			</view>
		</view>
		<view class="banner">
			<image src="../../static/images/caseBan.png" mode=""></image>
			<view class="text">
				<view class="t1">
				匠者之心·力求完美
				</view>
				<view class="t2">
					Craftsman's heart strives for perfection
				</view>
			</view>
		</view>


		<!-- 案例 -->
		<view class="cases">
			<view class="p1">
				<text class="t1">案例·</text>
				<text class="t2">cases</text>
			</view>
			<view class="p2">
				合理的要求是锻炼，不合理的要求是磨炼
			</view>
			<view class="allItems">
				<view class="item" v-for="(item,index) in caseList" :key="index">
					<view class="pic">
						<image :src="item.img" mode=""></image>
					</view>
					<view class="title">
						{{item.title}}
					</view>
					<view class="des">
						{{item.des}}
					</view>
				</view>
			</view>
			<view class="more">
				<text>更多案例</text>
				<image src="../../static/images/jiantou.png" mode=""></image>
			</view>
		</view>


		

	</view>
</template>

<script>
	export default {
		data() {
			return {
				caseList: [{
						img: require('../../static/images/c1.png'),
						title: '中核博浪集团',
						des: '网站策划 / 定制设计 / 前端开发 / 后台开发'
					},
					{
						img: require('../../static/images/c2.png'),
						title: '中核博浪集团',
						des: '网站策划 / 定制设计 / 前端开发 / 后台开发'
					}
				]
			}
		},
		onLoad() {
			
			uni.loadFontFace({
				family: 'HYQiHei-40S',
				source: 'url("http://test.nbtsm.cn/web/fonts/HYQiHei-40S.otf")',
				success(res) {
					console.log('获取字体成功')
				}
			})
			
			uni.loadFontFace({
				family: 'JM-Exposition Plain-One',
				source: 'url("http://test.nbtsm.cn/web/fonts/JM-Exposition Plain-One.ttf")',
				success(res) {
					console.log('获取字体成功')
				}
			})
			
			uni.loadFontFace({
				family: 'FZCYSK--GBK1-0',
				source: 'url("http://test.nbtsm.cn/web/fonts/FZCYSK--GBK1-0.TTF")',
				success(res) {
					console.log('获取字体成功')
				}
			})
			
			uni.loadFontFace({
				family: 'TimesNewRomanPSMT',
				source: 'url("http://test.nbtsm.cn/web/fonts/TimesNewRomanPSMT.otf")',
				success(res) {
					console.log('获取字体成功')
				}
			})

			uni.loadFontFace({
				family: 'SOURCEHANSANSCN-REGULAR',
				source: 'url("http://test.nbtsm.cn/web/fonts/SOURCEHANSANSCN-REGULAR.OTF")',
				success(res) {
					console.log('获取字体成功')
				}
			})
			
			uni.loadFontFace({
				family: 'SOURCEHANSANSCN-MEDIUM',
				source: 'url("http://test.nbtsm.cn/web/fonts/SOURCEHANSANSCN-MEDIUM.OTF")',
				success(res) {
					console.log('获取字体成功')
				}
			})

			uni.loadFontFace({
				family: 'MicrosoftYaHei',
				source: 'url("http://test.nbtsm.cn/web/fonts/MicrosoftYaHei.ttf")',
				success(res) {
					console.log('获取字体成功')
				}
			})
		},
		methods: {
		}
	}
</script>

<style lang="scss">
	.container {
		width: 100%;
		position: relative;
.header {
			width: 95%;
			position: fixed;
			left: 0;
			padding: 15px 2.5%;
			top: 0;
			display: flex;
			flex-direction: row;
			justify-content: space-between;
			align-items: center;
			z-index: 100;

			.logo {
				image {
					width: 187rpx;
					height: 60rpx;
				}
			}

			.contact {
				color: white;
				font-size: 24rpx;
				font-family: "SOURCEHANSANSCN-REGULAR";
			}
		}

		.banner {
			width: 100%;
			position: relative;
		
			image {
				width: 100%;
				height: 673rpx;
			}
			.text{
				position: absolute;
				left:0;
				top:50%;
				text-align: center;
				width:100%;
				transform: translateY(-50%);
		.t1 {
			color: white;
			font-size: 48rpx;
			font-family: 'FZCYSK--GBK1-0';
			letter-spacing: 15rpx;
		}
		
		.t2 {
			color: white;
			font-size: 20rpx;
			text-transform: uppercase;
			margin:20rpx 0;
			font-family: 'FZCYSK--GBK1-0';
		}
			}
		}

		.about {
			width: 95%;
			padding: 50rpx 2.5%;
			background-color: #EEEEEE;

			.title {
				width: 100%;

				.p1 {
					width: 100%;
					display: flex;
					flex-direction: row;
					justify-content: center;

					.t1 {
						font-weight: bolder;
						font-size: 60rpx;
						color: #535353;
						font-family: "FZCYSK--GBK1-0";
					}

					.t2 {
						font-size: 60rpx;
						color: #535353;
							font-family: "FZCYSK--GBK1-0";
					}
				}

				.en {
					color: #888888;
					font-size: 24rpx;
					margin: 10rpx 0;
					text-align: center;
					text-transform: uppercase;
						font-family: "FZCYSK--GBK1-0";
				}

				.pic {
					width: 100%;
					margin: 30rpx auto;

					image {
						width: 100%;
						display: block;
					}
				}

				.des {
					color: #333333;
					font-size: 28rpx;
					line-height: 55rpx;
					margin: 10rpx 0;
					font-family: "SOURCEHANSANSCN-REGULAR";
				}

				.more {
					width: 30%;
					background-color: #D20010;
					padding: 15rpx 20rpx;
					display: flex;
					flex-direction: row;
					align-items: center;
					margin: 30rpx auto;
					justify-content: center;

					text {
						color: white;
						font-size: 28rpx;
					}

					image {
						width: 35rpx;
						height: 7rpx;
						display: inline-block;
						margin-left: 10rpx;
					}
				}
			}
		}

		.solution {
			width: 100%;
			position: relative;

			.bgPic {
				width: 100%;
				display: block;
			}

			.content {
				position: absolute;
				left: 0;
				top: 0;
				width: 100%;
				height: 100%;
				display: flex;
				flex-direction: row;
				justify-content: space-between;

				.item {
					width: 33.3%;

					.oItem {
						width: 100%;
						display: flex;
						flex-direction: column;
						align-items: center;
						justify-content: center;
						height: 50%;
						border-bottom: 1px solid rgba($color: white, $alpha: .5);
						border-right: 1px solid rgba($color: white, $alpha: .5);

						.pic {
							image {
								max-width: 80rpx;
								max-height: 80rpx;
								object-fit: contain;
							}
						}

						.title {
							color: white;
							font-size: 30rpx;
							margin: 15rpx 0;
								font-family: "SOURCEHANSANSCN-REGULAR";
						}
					}
				}

				.item2 {
					width: 33.3%;
					display: flex;
					flex-direction: column;
					align-items: center;
					justify-content: center;

					.pic {
						image {
							max-width: 80rpx;
							max-height: 80rpx;
							object-fit: contain;
						}
					}

					.title {
						color: white;
						font-size: 30rpx;
							font-family: "SOURCEHANSANSCN-REGULAR";
					}
				}
			}
		}


		.cases {
			width: 95%;
			margin: 50rpx auto;

			.p1 {
				width: 100%;
				display: flex;
				flex-direction: row;
				justify-content: center;

				.t1 {
					font-weight: bolder;
					font-size: 60rpx;
					color: #535353;
					font-family: "FZCYSK--GBK1-0";
				}

				.t2 {
					font-size: 60rpx;
					color: #535353;
					text-transform: uppercase;
					font-family: "FZCYSK--GBK1-0";
				}
			}

			.p2 {
				color: #888888;
				font-size: 26rpx;
				margin: 15rpx 0;
				text-align: center;
							font-family: "FZCYSK--GBK1-0";
			}

			.allItems {
				width: 100%;
				margin: 30rpx auto;

				.item {
					width: 100%;
					margin-bottom: 40rpx;

					.pic {
						image {
							width: 100%;
							display: block;
							object-fit: cover;
						}
					}

					.title {
						color: #333333;
						font-size: 32rpx;
						margin: 20rpx 0 10rpx 0;
						font-family: "SOURCEHANSANSCN-MEDIUM";
					}

					.des {
						color: #666666;
						font-size: 24rpx;
						font-family: "SOURCEHANSANSCN-REGULAR";
					}
				}
			}

			.more {
				width: 30%;
				background-color: #D20010;
				padding: 15rpx 20rpx;
				display: flex;
				flex-direction: row;
				align-items: center;
				margin: 30rpx auto;
				justify-content: center;

				text {
					color: white;
					font-size: 28rpx;
				}

				image {
					width: 35rpx;
					height: 7rpx;
					display: inline-block;
					margin-left: 10rpx;
				}
			}
		}

		.partner {
			width: 95%;
			padding: 50rpx 2.5%;
			background-color: #EEEEEE;

			.p1 {
				width: 100%;
				display: flex;
				flex-direction: row;
				justify-content: center;

				.t1 {
					font-weight: bolder;
					font-size: 60rpx;
					color: #535353;
								font-family: "FZCYSK--GBK1-0";
				}

				.t2 {
					font-size: 60rpx;
					color: #535353;
					text-transform: uppercase;
								font-family: "FZCYSK--GBK1-0";
				}
			}

			.p2 {
				color: #888888;
				font-size: 26rpx;
				margin: 15rpx 0;
				text-align: center;
							font-family: "FZCYSK--GBK1-0";
			}

			.allPics {
				width: 100%;
				display: flex;
				flex-direction: row;
				flex-wrap: wrap;
				margin: 40rpx auto;
				position: relative;

				.line1 {
					width: 100%;
					height: 1px;
					position: absolute;
					top: 33.3%;
					left: 0;
					background-color: #EEEEEE;
				}

				.line2 {
					width: 100%;
					height: 1px;
					position: absolute;
					top: 66.6%;
					left: 0;
					background-color: #EEEEEE;
				}

				.line3 {
					width: 1px;
					height: 100%;
					position: absolute;
					top: 0;
					left: 33.3%;
					background-color: #EEEEEE;
				}

				.line4 {
					width: 1px;
					height: 100%;
					position: absolute;
					top: 0;
					left: 66.6%;
					background-color: #EEEEEE;
				}

				.item {
					width: 33.3%;
					background: #FFFFFF;
					display: flex;
					flex-direction: column;
					align-items: center;
					justify-content: center;
					padding: 30rpx 0;

					image {
						max-height: 50rpx;
						max-width: 150rpx;
						object-fit: contain;
					}
				}
			}
		}
	}
</style>
