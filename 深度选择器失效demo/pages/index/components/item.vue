<template>
  <view class="flex-row equal-division">
    <Child src="/static/logo.png" v-for="(item,index) in 4" :key="index"></Child>
    <!-- <u-image width="140rpx" height="140rpx" border-radius="12rpx" src="/static/logo.png" v-for="(item,index) in 4" :key="index">
    </u-image> -->
  </view>
</template>

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