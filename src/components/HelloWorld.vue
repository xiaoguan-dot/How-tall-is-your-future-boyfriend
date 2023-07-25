<script setup>
	import {
		ref
	} from 'vue'

	defineProps({
		msg: String
	})
	const count = ref(0);
	const cou = count.toString()  // id = "18"

	const wen = `https://www.baidu.com/s?tn=39042058_8_oem_dg&ie=utf-8&wd={{this.count}}cm 的男生现实多高啊?`;
</script>

<template>
	<h1>{{ msg }}</h1>
	<h5>(现在已经有的勿入...👉🏻👈🏻)</h5>

	<div class="card">
		<button type="button" @click="count++">你未来男朋友 {{ count }}cm 高</button>
		<p class="read-the-docs">
			偷偷告诉你 按
			<code>F12或Fn+F12</code> 可以直接修改未来男朋友滴高度 👌
		</p>
	</div>

	<p>
		偷偷问下度娘！
		<a :href="wen" target="_blank">
			{{ count }}cm 的男生现实多高啊！</a>
	</p>
	<p>
		看小编已经这么努力啦~能给这个Hello World 哦不给小编
		<a href="https://baike.baidu.com/item/%E5%8A%A0%E9%B8%A1%E8%85%BF/22206583" target="_blank">加个鸡腿吗？</a>
		<a @click="thank++">肯定要加啊~</a>
	</p>
	<p class="read-the-docs">By Xiaoguan <br>小关之作</p>
</template>

<style scoped>
	.read-the-docs {
		color: #888;
	}
</style>