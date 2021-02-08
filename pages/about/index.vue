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
			<image src="../../static/images/abanner.png" mode=""></image>
			<view class="text">
				<view class="t1">
					专注·创意设计
				</view>
				<view class="t2">
					focus on creative design, original
				</view>
			</view>
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
					万千星网络创立于2009年，是一家专注于高端网站建设、技术开发和品牌传播的网络服务机构，致力于为企业提供全面、丰富的网络解决方案。在网站建设创意提升、软件开发技术革新、品牌传播效果提升方面拥有着丰富经验。公司通过建立对目标客户和用户行为的分析，凭借网站建设、网站设计创意出众，精准把握企业对国内国外网站制作，海外网站设计的实际需求，打造创意十足、有价值的视觉体验，并以全球化进程为目标，为企业提供全方位的网络服务，包括APP、h5、微信、小程序设计开发，电商、平台、软件设计开发、海内海外内容营销、口碑维护、网络传播。技术优秀、传播高效，15年来积极探索并不断创新，坚持为合作伙伴创造更多惊喜
				</view>
			</view>
			<view class="nums">
				<view class="item">
					<view class="onum">
						<text>10</text>
						<text>年</text>
					</view>
					<view class="t">
						行业实战经验
					</view>
				</view>

				<view class="item">
					<view class="onum">
						<text>1000</text>
						<text>+</text>
					</view>
					<view class="t">
						客户选择
					</view>
				</view>

				<view class="item">
					<view class="onum">
						<text>112</text>
						<text>+</text>
					</view>
					<view class="t">
						细节标准
					</view>
				</view>
			</view>
		</view>


		<!-- 为什么选择我们 -->
		<view class="chose">
			<view class="bgPic">
				<image src="../../static/images/aBg.png" mode="widthFix"></image>
			</view>
			<view class="text">
				<view class="t1">
					为什么选择我们
				</view>
				<view class="t2">
					设计只是表象，在设计背后，是对消费心理的深刻洞察，<br>
					是对商业模式的深入思考，是对定位的精准考量<br>
					是对产品的解构与重构。
				</view>
				<view class="pic">
					<image src="../../static/images/ab.png" mode=""></image>
				</view>
			</view>
		</view>

		<!-- 服务领域 -->
		<view class="service">
			<view class="text">
				<view class="t1">
					我们的服务领域
				</view>
				<view class="t2">
					Our service areas
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

<!-- 服务优势 -->
<view class="advantage">
	<view class="bgPic">
		<image src="../../static/images/fbg.png" mode="widthFix"></image>
	</view>
	<view class="text">
		<view class="t1">
			服务优势
		</view>
		<view class="t2">
		以品牌为导向、数字平台营销的理念对网站进行整体构建
		</view>
	</view>
	<view class="allItems">
		<view class="item1">
			<image src="../../static/images/circle.png"></image>
			<view class="st">
				<view class="s1">专注</view>
				<view class="s2">Focus</view>
			</view>
		</view>
		<view class="item1">
			<image src="../../static/images/circle.png"></image>
			<view class="st">
				<view class="s1">创新</view>
				<view class="s2">Innovation</view>
			</view>
		</view>
		<view class="item1">
			<image src="../../static/images/circle.png"></image>
			<view class="st">
				<view class="s1">品质</view>
				<view class="s2">Quality</view>
			</view>
		</view>
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

			.nums {
				width: 100%;
				margin: 60rpx auto;
				display: flex;
				flex-direction: row;
				justify-content: space-between;

				.item {
					width: 30%;
					text-align: center;

					.onum {
						position: relative;

						text:nth-child(1) {
							color: #333333;
							font-size: 61rpx;
							font-family: "FZCYSK--GBK1-0";
						}

						text:nth-child(2) {
							font-size: 20rpx;
							color: #AAAAAA;
							font-family: "FZCYSK--GBK1-0";
						}
					}

					.t {
						color: #AAAAAA;
						font-size: 24rpx;
						font-family: "SOURCEHANSANSCN-REGULAR";
						margin: 20rpx auto;
					}
				}
			}
		}

		.chose {
			width: 100%;
			padding: 100rpx 0;
			position: relative;
			.bgPic{
				width:100%;
				top:0;
				height:100%;
				position: absolute;
				left:0;
				z-index: -1;
				image{
					width:100%;
				}
			}

			.text {
				text-align: center;
				width: 90%;
				margin: 0 auto;

		    .t1 {
					color: white;
					font-size: 48rpx;
					font-family: "FZCYSK--GBK1-0";
				}

				.t2 {
					color: white;
					font-size: 23rpx;
					font-family: "SOURCEHANSANSCN-REGULAR";
					margin: 40rpx 0;
					line-height: 20px;
				}

				.pic {
					width: 90%;
					margin: 60rpx auto;

					image {
						width: 100%;
						display: block;
						object-fit: contain;
						height: 370rpx;
					}
				}
			}
		}
        .service{
			width:95%;
			margin: 60rpx auto;
			.text{
				width:100%;
				text-align: center;
				.t1{
					color:#222222;
					font-size: 48rpx;
					font-family: "FZCYSK--GBK1-0";
				}
				.t2{
					color:#888888;
					font-family: "FZCYSK--GBK1-0";
					font-size: 24rpx;
					margin: 15rpx auto;
				}
			}
			.allItems{
				width:100%;
				display: flex;
				flex-direction: row;
				flex-wrap: wrap;
				justify-content: space-between;
				margin: 60rpx auto;
				.item{
					width:49%;
					background-color: #272B3D;
					text-align: center;
					padding: 40rpx 0;
					.pic{
						width:100rpx;
						height:100rpx;
						display: flex;
						flex-direction: column;
						align-items: center;
						justify-content: center;
						margin: 0 auto;
					}
					.title{
						color:white;
						font-size: 24rpx;
						margin: 10rpx auto;
						font-family: "SOURCEHANSANSCN-REGULAR";
					}
				}
				.item:nth-child(1){
					.pic{
						image{
							width:78rpx;
							height:56rpx;
							object-fit: contain;
						}
					}
				}
				.item:nth-child(2){
					.pic{
						image{
							width:48rpx;
							height:84rpx;
							object-fit: contain;
						}
					}
				}
				.item2{
					width:32%;
					background-color: #E5E5E5;
					text-align: center;
					padding: 40rpx 0;
					margin-top: 15rpx;
					.pic{
						width:100rpx;
						height:100rpx;
						display: flex;
						flex-direction: column;
						align-items: center;
						justify-content: center;
						margin: 0 auto;
						image{
							width:80rpx;
							height:80rpx;
							object-fit: contain;
						}
					}
					.title{
						font-size: 24rpx;
						margin: 10rpx auto;
						font-family: "SOURCEHANSANSCN-REGULAR";
					}
				}
			}
		}

.advantage{
	width:100%;
	padding: 80rpx 0;
	position: relative;
	.bgPic{
		width:100%;
		top:0;
		height:100%;
		position: absolute;
		left:0;
		z-index: -1;
		image{
			width:100%;
		}
	}
	.text{
		width:90%;
		margin: 0 auto;
		text-align: center;
		.t1{
			color:white;
			font-size: 48rpx;
			font-family: "FZCYSK--GBK1-0";
		}
		.t2{
			color:white;
					font-family: "FZCYSK--GBK1-0";
					font-size: 24rpx;
					opacity: .5;
					margin: 20rpx 0;
		}
	}
	.allItems{
		width:90%;
		margin: 60rpx auto;
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		justify-content: center;
		.item1{
			width:40%;
			position: relative;
			image{
				width:257rpx;
				height:254rpx;
				object-fit: contain;
			}
			.st{
				position: absolute;
				left:50%;
				top:50%;
				transform: translate(-45%,-50%);
				text-align: center;
				.s1{
					color:white;
					font-size: 36rpx;
					font-family: "FZCYSK--GBK1-0";
				}
				.s2{
					color:white;
					font-size: 22rpx;
					font-family: "FZCYSK--GBK1-0";
					text-transform: uppercase;
					margin-top: 10rpx;
				}
			}
		}
		.item1:nth-child(1){
			width:100%;
			text-align: center;
		}
		.item1:not(:first-child){
			margin: 0 2%;
		}
	}
}
		.partner {
			width: 95%;
			padding: 80rpx 2.5%;
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
