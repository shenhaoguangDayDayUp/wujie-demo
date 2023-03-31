<template>
  <!--单例模式，name相同则复用一个无界实例，改变url则子应用重新渲染实例到对应路由 -->
  <WujieVue width="100%" height="100%" name="vite-vue3" :url="viteUrl"></WujieVue>
</template>

<script>
import hostMap from "../hostMap";

export default {
  computed: {
    viteUrl() {
      return hostMap("//localhost:8100/")
    },
  },
};
</script>

<style lang="scss" scoped></style>
