<template>
	<view class="container">

		<!-- 顶部 -->
		<view class="header">
			<view class="logo">
				<image src="../../static/images/logo.png" mode=""></image>
			</view>
		</view>

		<!-- 轮播 -->
		<view class="banner">
			<image src="../../static/images/shopBan.png" mode=""></image>
			<view class="text">
				<view class="t1">
					开拓创新·行稳致远
				</view>
				<view class="t2">
					Pioneering and innovative steady and far-reaching
				</view>
			</view>
		</view>

		<!-- 服务领域 -->
		<view class="service">
			<view class="text">
				<view class="t1">
					致力于企业品牌形象建设和传播
				</view>
				<view class="t2">
					多年来，万千星网络不忘初心，以建立行业服务标杆为目标，不断提升技术设计服务水平，帮助客户在互联网推广自己的产品、服务和品牌，为客户创造价值从而实现自身价值！
				</view>
			</view>
			<view class="allItems">
				<view class="item">
					<view class="pic">
						<image src="../../static/images/web.png" mode=""></image>
					</view>
					<view class="title">
						网站建设
					</view>
				</view>
				<view class="item">
					<view class="pic">
						<image src="../../static/images/mini.png" mode=""></image>
					</view>
					<view class="title">
						小程序公众号开发
					</view>
				</view>
				<view class="item2">
					<view class="pic">
						<image src="../../static/images/shop.png" mode="widthFix"></image>
					</view>
					<view class="title">
						商城门户
					</view>
				</view>
				<view class="item2">
					<view class="pic">
						<image src="../../static/images/sys.png" mode="widthFix"></image>
					</view>
					<view class="title">
						系统软件
					</view>
				</view>
				<view class="item2">
					<view class="pic">
						<image src="../../static/images/inter.png" mode="widthFix"></image>
					</view>
					<view class="title">
						网络营销
					</view>
				</view>
			</view>
		</view>

		<!-- 积累拥抱新技术 -->
		<view class="tech">
			<view class="bgPic">
				<image src="../../static/images/tBg.png" mode="widthFix"></image>
			</view>
			<view class="text">
				<view class="t1">
					积极拥抱新技术
				</view>
				<view class="t2">
					探索新领域
				</view>
				<view class="t3">
					展示型网站建设、B2B供需平台开发、在线教育平台开发...
				</view>
			</view>
		</view>


		<!-- 选择 -->
		<view class="chose">
			<view class="title">
				<view class="t1">
					选择万千星 品牌保证
				</view>
				<view class="t2">
					洞察用户需求与商业价值，帮客户打造极致体验的产品并创造价值
				</view>
			</view>
			<view class="allItems">
				<view class="item" v-for="(item,index) in list" :key="index">
					<view class="st">
						0{{index+1}}
					</view>
					<view class="t1">
						{{item.title}}
					</view>
					<view class="t2">
						{{item.des}}
					</view>
				</view>
			</view>
		</view>


		<!-- 服务流程 -->
		<view class="fuwu">
			<view class="bgPic">
				<image src="../../static/images/fuwuBg.png"></image>
			</view>
			<view class="content">
				<view class="title">
					<view class="t1">
						服务流程
					</view>
					<view class="t2">
						一站式的品牌数字服务体系，助力品牌全流程价值提升
					</view>
				</view>
				<view class="allItems">
					<view class="item" v-for="(item,index) in sList" :key="index">
						<view class="pic">
							<image :src="item.img"></image>
						</view>
						<view class="text">
							<view class="circle">
								<view></view>
							</view>
							<view class="t">
								{{item.title}}
							</view>
						</view>
					</view>
				</view>
			</view>
		</view>

	</view>
</template>

<script>
	export default {
		data() {
			return {
				sList: [{
						img: require('../../static/images/fwlc01.png'),
						title: '策划'
					},
					{
						img: require('../../static/images/fwlc01.png'),
						title: '策划'
					},
					{
						img: require('../../static/images/fwlc01.png'),
						title: '策划'
					},
					{
						img: require('../../static/images/fwlc01.png'),
						title: '策划'
					},
					{
						img: require('../../static/images/fwlc01.png'),
						title: '策划'
					},
					{
						img: require('../../static/images/fwlc01.png'),
						title: '策划'
					},
					{
						img: require('../../static/images/fwlc01.png'),
						title: '策划'
					}
				],
				list: [{
						title: '系统解决方案',
						des: '我们提供多项系统解决方案，满足不同业务的开发需求'
					},
					{
						title: '系统解决方案',
						des: '我们提供多项系统解决方案，满足不同业务的开发需求'
					},
					{
						title: '系统解决方案',
						des: '我们提供多项系统解决方案，满足不同业务的开发需求'
					},
					{
						title: '系统解决方案',
						des: '我们提供多项系统解决方案，满足不同业务的开发需求'
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
				family: 'SOURCEHANSANSCN-HEAVY',
				source: 'url("http://test.nbtsm.cn/web/fonts/SOURCEHANSANSCN-HEAVY.OTF")',
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
		methods: {}
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
		}

		.banner {
			width: 100%;
			position: relative;

			image {
				width: 100%;
				height: 673rpx;
			}

			.text {
				position: absolute;
				left: 0;
				top: 50%;
				text-align: center;
				width: 100%;
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

		.service {
			width: 95%;
			margin: 60rpx auto;

			.text {
				width: 100%;

				.t1 {
					color: #222222;
					font-size: 36rpx;
					font-family: "SOURCEHANSANSCN-HEAVY";
				}

				.t2 {
					color: #666666;
					font-family: "SOURCEHANSANSCN-REGULAR";
					font-size: 22rpx;
					margin: 25rpx auto;

				}
			}

			.allItems {
				width: 100%;
				display: flex;
				flex-direction: row;
				flex-wrap: wrap;
				justify-content: space-between;
				margin: 60rpx auto;

				.item {
					width: 49%;
					background-color: #272B3D;
					text-align: center;
					padding: 40rpx 0;

					.pic {
						width: 100rpx;
						height: 100rpx;
						display: flex;
						flex-direction: column;
						align-items: center;
						justify-content: center;
						margin: 0 auto;
					}

					.title {
						color: white;
						font-size: 24rpx;
						margin: 10rpx auto;
						font-family: "SOURCEHANSANSCN-REGULAR";
					}
				}

				.item:nth-child(1) {
					.pic {
						image {
							width: 78rpx;
							height: 56rpx;
							object-fit: contain;
						}
					}
				}

				.item:nth-child(2) {
					.pic {
						image {
							width: 48rpx;
							height: 84rpx;
							object-fit: contain;
						}
					}
				}

				.item2 {
					width: 32%;
					background-color: #E5E5E5;
					text-align: center;
					padding: 40rpx 0;
					margin-top: 15rpx;

					.pic {
						width: 100rpx;
						height: 100rpx;
						display: flex;
						flex-direction: column;
						align-items: center;
						justify-content: center;
						margin: 0 auto;

						image {
							width: 80rpx;
							height: 80rpx;
							object-fit: contain;
						}
					}

					.title {
						font-size: 24rpx;
						margin: 10rpx auto;
						font-family: "SOURCEHANSANSCN-REGULAR";
					}
				}
			}
		}

		.tech {
			position: relative;
			width: 100%;
			background-color: #eeeeee;

			.bgPic {
				width: 100%;

				image {
					width: 100%;
				}
			}

			.text {
				width: 90%;
				left: 5%;
				top: 20%;
				position: absolute;

				.t1 {
					color: white;
					font-size: 34rpx;
					font-family: "SOURCEHANSANSCN-REGULAR";
				}

				.t2 {
					color: white;
					font-size: 48rpx;
					font-family: "FZCYSK--GBK1-0";
					position: relative;
					padding-bottom: 50rpx;
					margin-top: 10rpx;

					&::after {
						width: 81rpx;
						height: 4rpx;
						content: '';
						display: inline-block;
						position: absolute;
						bottom: 0;
						left: 0;
						background-color: white;
					}
				}

				.t3 {
					color: white;
					font-size: 16rpx;
					font-family: "SOURCEHANSANSCN-REGULAR";
					margin-top: 180rpx;
				}
			}
		}

		.chose {
			background-color: #eeeeee;
			width: 100%;
			padding: 60rpx 0;

			.title {
				width: 95%;
				margin: 0 auto;
				text-align: center;

				.t1 {
					color: #535353;
					font-size: 48rpx;
					font-family: "FZCYSK--GBK1-0";
				}

				.t2 {
					color: #888888;
					font-size: 24rpx;
					font-family: "FZCYSK--GBK1-0";
					margin: 20rpx auto;

				}
			}

			.allItems {
				width: 95%;
				margin: 60rpx auto;

				.item {
					width: 90%;
					padding: 80rpx 5%;
					background-color: white;
					position: relative;
					margin-bottom: 30rpx;

					.st {
						position: absolute;
						right: 5%;
						top: 30rpx;
						color: #E9E9E9;
						font-size: 48rpx;
						font-family: "FZCYSK--GBK1-0";
					}

					.t1 {
						color: #333333;
						font-size: 28rpx;
						font-family: "SOURCEHANSANSCN-REGULAR";
					}

					.t2 {
						color: #666666;
						font-size: 20rpx;
						font-family: "SOURCEHANSANSCN-REGULAR";
						margin-top: 10rpx;
					}
				}
			}
		}

		.fuwu {
			width: 100%;
			position: relative;

			.bgPic {
				width: 100%;

				image {
					width: 100%;
					display: block;
					object-fit: contain;
					height: 884rpx;
				}
			}

			.content {
				width: 100%;
				position: absolute;
				left: 0;
				top: 15%;

				.title {
					width: 90%;
					margin: 0 auto;
					text-align: center;

					.t1 {
						color: white;
						font-size: 48rpx;
						font-family: "FZCYSK--GBK1-0";
					}

					.t2 {
						color: white;
						font-size: 24rpx;
						font-family: "FZCYSK--GBK1-0";
						margin: 30rpx 0;
					}
				}

				.allItems {
					width: 95%;
					display: flex;
					flex-direction: row;
					justify-content: space-between;
					position: relative;
					margin: 60rpx auto;
					margin-top: 160rpx;

					.item {
						display: flex;
						flex-direction: column;
						align-items: center;
						justify-content: center;
						z-index: 10;

						.pic {
							width: 76rpx;
							height: 76rpx;
							border-radius: 50%;
							background-color: #8C111B;
							display: flex;
							flex-direction: column;
							align-items: center;
							justify-content: center;
							transition: all 600ms;

							image {
								max-width: 40rpx;
								max-height: 40rpx;
								object-fit: contain;
							}
						}

						.text {
							font-family: 'MicrosoftYaHei';
							position: relative;
							transition: all 600ms;
							display: flex;
							flex-direction: column;
							align-items: center;
							justify-content: center;

							.circle {
								width: 13rpx;
								height: 13rpx;
								border: 1px solid rgba(255, 255, 255, .6);
								border-radius: 50%;
								position: relative;
								transition: all 600ms;
								margin: 30rpx 0;
     &::before,&::after{
                content:'';
                display: inline-block;
                width:66rpx;
                height:1px;
                background-color: white;
                position: absolute;
              }
              &::before{
                content:'';
                display: inline-block;
                left:0;
                top:50%;
                transform: translateY(-50%);
              }
              &::after{
                content:'';
                display: inline-block;
                right:0;
                top:50%;
                transform: translateY(-50%);
              }
								view {
									display: block;
									position: absolute;
									left: 50%;
									top: 50%;
									transform: translate(-50%, -50%);
									width: 60%;
									height: 60%;
									background-color: white;
									border-radius: 50%;
									opacity: 0;
									transition: all 600ms;
								}
							}
						.t{
							  opacity: .54;
							              color:white;
							              font-family: 'MicrosoftYaHei';
							              font-size: 22rpx;
						}
						}
					}
				}
			}
		}
	}
</style>
