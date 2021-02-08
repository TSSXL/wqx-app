<template>
	<view class="container">

		<!-- 顶部 -->
		<view class="header">
			<view class="logo">
				<image src="../../static/images/logo.png" mode=""></image>
			</view>
			<view class="contact" @click="gotoContact">
				联系我们
			</view>
		</view>
		<!-- 轮播 -->
		<view class="banner">
			<swiper class="swiper" :indicator-dots="indicatorDots" :autoplay="autoplay" :interval="interval" :duration="duration">
				<swiper-item v-for="(item,index) in banner" :key="index">
					<view class="pic">
						<image :src="item.img" mode=""></image>
						<view class="text">
							<view class="t1">
								{{item.t1}}
							</view>
							<view class="t2">
								{{item.t2}}
							</view>
							<view class="t3">
								{{item.t3}}
							</view>
							<view class="t4">
								{{item.t4}}
							</view>
						</view>
					</view>
				</swiper-item>
			</swiper>
		</view>

		<!-- 关于我们 -->
		<view class="about">
			<view class="title">
				<view class="p1">
					<text class="t1">关于·</text>
					<text class="t2">万千星</text>
				</view>
				<view class="en">
					who are we?
				</view>
				<view class="pic">
					<image src="../../static/images/about.png" mode=""></image>
				</view>
				<view class="des">
					宁波万千星网络技术有限公司是一家专业从事网站建设、网络推广、营销策划为一体的互联网公司。我公司技术团队力量雄厚，辅助于天津各个中小型企业网络推广营销。
					万千星网络自创立以来始终专注于网络品牌整合与创新设计，拥有严谨实用的设计体系，汇聚了品牌策略专家，创意设计专家，网络营销专家，公司致力于为您的企业提供专业的品牌策划、网站设计，网络营销等一站式解决方案，为您的企业提供一体化营销,高端网络品牌宣传。
				</view>
				<view class="more">
					<text>查看更多</text>
					<image src="../../static/images/jiantou.png" mode=""></image>
				</view>
			</view>
		</view>

		<!-- 五个解决方案 -->
		<view class="solution">
			<image class="bgPic" src="../../static/images/sbg.png" mode=""></image>
			<view class="content">
				<view class="item">
					<view class="oItem">
						<view class="pic">
							<image src="../../static/images/s1.png" mode=""></image>
						</view>
						<view class="title">
							网站建设
						</view>
					</view>
					<view class="oItem">
						<view class="pic">
							<image src="../../static/images/s2.png" mode=""></image>
						</view>
						<view class="title">
							商城门户
						</view>
					</view>
				</view>

				<view class="item">
					<view class="oItem">
						<view class="pic">
							<image src="../../static/images/s3.png" mode=""></image>
						</view>
						<view class="title">
							小程序开发
						</view>
					</view>
					<view class="oItem">
						<view class="pic">
							<image src="../../static/images/s4.png" mode=""></image>
						</view>
						<view class="title">
							系统软件
						</view>
					</view>
				</view>


				<view class="item2">
					<view class="pic">
						<image src="../../static/images/s5.png" mode=""></image>
					</view>
					<view class="title">
						网络营销
					</view>
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

		<!-- 合作伙伴 -->
		<view class="partner">
			<view class="p1">
				<text class="t1">伙伴·</text>
				<text class="t2">partner</text>
			</view>
			<view class="p2">
				许多人信任我们，获益良多，感谢伴随我们成长
			</view>
			<view class="allPics">
				<view class="line1">

				</view>
				<view class="line2">

				</view>
				<view class="line3">

				</view>
				<view class="line4">

				</view>
				<view class="item" v-for="(item,index) in pList" :key="index">
					<image :src="item.img" mode=""></image>
				</view>
			</view>
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
				duration: 1000,
				banner: [{
						img: require('../../static/images/banner.png'),
						t1: '触及视频灵魂的设计趋势',
						t2: 'vanchsun',
						t3: '因为高端·所以出众',
						t4: 'Outstanding because of high-end'
					},
					{
						img: require('../../static/images/banner.png'),
						t1: '触及视频灵魂的设计趋势',
						t2: 'vanchsun',
						t3: '因为高端·所以出众',
						t4: 'Outstanding because of high-end'
					}
				],
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
				],
				pList: [{
						img: require('../../static/images/p1.png')
					},
					{
						img: require('../../static/images/p1.png')
					},
					{
						img: require('../../static/images/p1.png')
					},
					{
						img: require('../../static/images/p1.png')
					},
					{
						img: require('../../static/images/p1.png')
					},
					{
						img: require('../../static/images/p1.png')
					},
					{
						img: require('../../static/images/p1.png')
					},
					{
						img: require('../../static/images/p1.png')
					},
					{
						img: require('../../static/images/p1.png')
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
			gotoContact() {
				uni.navigateTo({
					url: '../contact/index'
				})
			}
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
			height: 674rpx;

			.swiper {
				width: 100%;
				height: 674rpx;

				.pic {
					width: 100%;
					heiht: 100%;
					position: relative;

					.text {
						position: absolute;
						left: 0;
						top: 50%;
						transform: translateY(-50%);
						text-align: center;
						width: 100%;

						.t1 {
							color: #F39800;
							font-size: 30rpx;
							font-family: "HYQiHei-40S";
							letter-spacing: 8rpx;
						}

						.t2 {
							font-size: 114.82rpx;
							color: white;
							text-transform: uppercase;
							margin: 20rpx 0;
							font-family: "JM-Exposition Plain-One";
								letter-spacing: 15rpx;
						}

						.t3 {
							color: white;
							font-size: 36rpx;
							font-family: "FZCYSK--GBK1-0";
								letter-spacing: 8rpx;
						}

						.t4 {
							color: #FFFFFF;
							font-size: 16rpx;
							text-transform: uppercase;
							margin-top: 10rpx;
							font-family: "FZCYSK--GBK1-0";
								letter-spacing: 8rpx;
						}
					}

					image {
						width: 100%;
						height: 674rpx;
					}
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
