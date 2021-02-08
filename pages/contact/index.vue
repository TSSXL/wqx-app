<template>
	<view class="container">
		<!-- 顶部 -->
		<view class="header">
			<view class="logo">
				<image src="../../static/images/logo.png" mode=""></image>
			</view>
		</view>

		<view class="banner">
			<image src="../../static/images/cbanner.png" mode=""></image>
			<view class="text">
				<view class="t1">
					Hello,终于等到您来!
				</view>
				<view class="t2">
					Hello, finally waiting for you!
				</view>
			</view>
		</view>


<view class="main">
	<view  class="t1">
		联系我们
	</view>
	<view class="item">
		<view class="st">
			 公司名称
		</view>
		<view class="st2">
			宁波万千星网络有限公司
		</view>
	</view>
	
	<view class="item">
		<view class="st">
			 技术支持
		</view>
		<view class="st2">
	133-3686-4504
		</view>
	</view>
	
	<view class="item">
		<view class="st">
			商务咨询
		</view>
		<view class="st2">
			158-8816-7800
		</view>
	</view>
	
	<view class="item">
		<view class="st">
			邮箱地址
		</view>
		<view class="st2">
			info@wqxweb.com
		</view>
	</view>
	
	
	<view class="item">
		<view class="st">
		联系地址
		</view>
		<view class="st2">
		宁波市鄞州区学士路642弄2号卓悦大厦21楼
		</view>
	</view>
	
</view>

	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		onLoad() {
	      	uni.loadFontFace({
	      		family: 'FZCYSK--GBK1-0',
	      		source: 'url("http://test.nbtsm.cn/web/fonts/FZCYSK--GBK1-0.TTF")',
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
		
		.main{
			width:90%;
			margin: 40rpx auto;
			.t1{
				color:#333333;
				font-size: 48rpx;
				font-family: "SOURCEHANSANSCN-REGULAR";
			}
			.item{
				margin-top: 30rpx;
				.st{
					font-size: 22rpx;
					font-family: "MicrosoftYaHei";
				}
				.st2{
					font-size: 28rpx;
					margin-top: 10rpx;
					font-family: "MicrosoftYaHei";
				}
			}
		}
	}
</style>
