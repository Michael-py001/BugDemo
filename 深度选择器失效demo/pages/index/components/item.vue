<template>
  <view class="flex-row equal-division">
    <Child src="/static/logo.png" v-for="(item,index) in 4" :key="index"></Child>
  </view>
</template>

<script >
  export default {
     options: {
        styleIsolation: 'shared'
      }
  }
</script>

<script setup>
  import Child from './Child'
</script>

<style lang="scss">
  .equal-division {
       margin-top: 22rpx;
       ::v-deep .my-image {
         margin-right: 27rpx;
       }
     }
</style>