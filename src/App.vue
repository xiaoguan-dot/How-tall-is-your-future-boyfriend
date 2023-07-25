<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div>
    <a href="https://xiaoguan.fit" target="_blank">
      <img src="/xiaoguan.svg" class="logo" alt="Xiaoguan logo" />
    </a>
	      
    <a href="https://douyin.com/" target="_blank">
      <img src="/douyind.svg" class="logo vue" alt="Douyin logo" />
    </a>
  </div>
  <HelloWorld msg="你未来男朋友长多高🤣🤣" />
</template>
ds
<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #1D9BF0);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #ff0050);
}
</style>
