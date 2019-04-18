<template>
<view class="containner">
		<view class="topper"></view>
		<view class="top">
			<text class="top-title">关注</text>
			<image class="tianjia" src="../../static/add.png"></image>
			<image class="sousuo" src="../../static/find.png"></image>
		</view>
		<view class="sec-top"><image src="../../static/top2.jpg"></image></view>
		<view class="divide"></view>
		<view class="bigcard">
			<view class="card" v-for="(book, index) in books" :key="index">
				<view class=" txcard"><img class="touxiang" :src="book.cover" /></view>
				<view class=" fontcard">
					
					<span class="ko titfont">{{ book.title }}</span>
					<br />
					<span class="ko word">{{ book.word }}</span>
					
				</view>
			</view>
		</view>
		<view class="bottom"><image src="../../static/bottom.png"></image></view>
	</view>
	
</template>

<script>
export default {
		data() {
			return {
				books: [
					{
						title: '陶然然_niit',
						word: '7 Spring Boot项目打包运行',
						cover: 'static/1.jpg',
					
						
					},
					{
						title: '六年的承诺',
						word: '实现蓝墨云',
						cover: 'static/2.jpg',
						
					},
					{
						title: '1只念旧的兔子',
						word: 'SpringBoot和MyBatis的集成练习',
						cover: 'static/3.jpg',
						
					},
					{
						title: '七夏港_f3ef',
						word: '6.SpringBoot打包',
						cover: 'static/4.jpg',
						
					},
					{
						title: '次饭饭_2628',
						word: 'Spring Boot起步',
						cover: 'static/5.jpg',
						
					},
					{
						title: '洋baby',
						word: '4.一个两表关联查询的例子',
						cover: 'static/6.jpg',
						
					},
					{
						title: 'm小萌同学',
						word: 'SPA:单页应用',
						cover: 'static/7.jpg',
						
					}
				]
				
			};
		},
		onLoad() {},
		methods: {}
	};
</script>

<style>
.divide {
	width: 100%;
	height: 20upx;
	}
.title {
	font-size: 36upx;
	
}
.sec-top {
	width: 100%;
	height: 100upx;
}
.sec-top image {
	width: 100%;
	height: 90%;
}

.touxiang {
	width: 52px;
	height: 52px;
	border-radius: 5px;
	margin: 0 auto;
}
.fontcard {
	width: 270px;
	height: 52px;
	border-top: 0px;
	border-right: 0px;
	border-left: 0px;
	border-bottom: #e6e6e6 0.2px solid;
	margin-left: 150upx;
	margin-top: 10px;
}
.txcard {
	width: 52px;
	height: 55px;
	float: left;
	margin-top: 10px;
}
.sousuo {
	width: 50upx;
	height: 50upx;
	float: right;
	margin-right: 20px;
}
.caifua {
	width: 50upx;
	height: 50upx;
	float: right;
	margin-right: 13px;
}
.tianjia {
	width: 58upx;
	height: 58upx;
	float: left;
	margin-left: 5px;
}
.word {
	font-size: 14px;
	color: darkgray;
}
.titfont {
	font-size: 17px;
}

.bigcard {
	width: 100%;
	height: 450px;
	border-color: #a9a9a9;
}

.card {
	text-align: left;
	padding-top: 5px;
	margin-left: 10px;
	margin-right: 10px;
	font-size: 14px;
	line-height: 25px;
}
.top {
	height: 50upx;
	width: 100%;
	padding-top: 11px;
}
.top-title {
	font-size: 18px;
	color: darkgray;
}
.topper {
	width: 100%;
	height: 60upx;
}
.bottom {
	width: 100%;
	height: 150px;
}
.bottom image {
	width: 100%;
	height: 100%;
}

</style>
