<template>
  <image class="my-image" :src="src" mode="aspectFill"></image>
</template>


<script setup>
  const props = defineProps({
    src:String
  })
</script>

<style lang="scss" scoped>
  .my-image {
    width: 100rpx;
    height: 100rpx;
  }
</style>