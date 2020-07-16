<template>
	<view class="content">
		<!-- <image class="logo" src="/static/logo.png"></image>
		<view>
			<text class="title">{{title}}</text>
		</view> -->
		<view class='person-info'>
			<view class="info-name-setting">
				<view class="info-name">
					<image class='info-img' :src="img"></image>
					<view class='info-name-name'>
						<view class="info-name-text">{{name}}</view>
						<view class="info-name-lv">{{level}}</view>
					</view>
				</view>
				<view class="info-setting">
					<image class="setting-img setting-icon" :src='img'></image>
					<image class="setting-img" :src='img'></image>
				</view>
			</view>
			<view class="info-list">
				<view class='info-item' v-for="item in myList">
					<image class='info-item-image' :src="item.img" alt=''></image>
					<view class='info-item-text'>{{item.text}}</view>
				</view>
			</view>
		</view>
		<view class= 'person-list'></view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello',
				img:'/static/logo.png',
				name:'刘敏敏',
				level:'LV7',
				setting:'',
				myList:[
					{img:'/static/logo.png',text:'我的权益',link:''},
					{img:'/static/logo.png',text:'我的积分',link:''},
					{img:'/static/logo.png',text:'我的红包',link:''},
				]
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	@import url("./index.less");
</style>
