<template>
	<view class="content">
		<upload-demo type="image" :list="fileList" disabled></upload-demo>
		<upload-demo type="image" ></upload-demo>
		<upload-demo type="video"></upload-demo>
		<!-- #ifdef H5 || APP-PLUS || MP-WEIXIN -->
		<upload-demo type="file"></upload-demo>
		<!-- #endif -->
	</view>
</template>

<script>
import UploadDemo from '@/components/UploadDemo';

export default {
	components: {
		UploadDemo,
	},
	data() {
		return {
			fileList: [
				{
					"fileName": "shuijiao.jpg",
					"fileKey": "7c524b43bf1ff89aeda1eb439aad3268.jpg",
					"filePath": "https://web-assets.dcloud.net.cn/unidoc/zh/shuijiao.jpg",
					"url": "https://web-assets.dcloud.net.cn/unidoc/zh/shuijiao.jpg",
					"name": "shuijiao.jpg",
					"fileType": "image"
				}
			]
		};
	},
	onLoad() {},
	methods: {},
};
</script>

<style>
.content {
	padding: 32rpx 0;
}
</style>
