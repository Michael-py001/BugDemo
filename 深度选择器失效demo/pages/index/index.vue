<template>
	<view class="content">
		<Item></Item>
	</view>
</template>

<script setup>
  import Item from './components/item'
</script>

<style lang="scss">
  .flex-row {
    display: flex;
    flex-direction: row;
  }
  .equal-division {
       margin-top: 22rpx;
       // ::v-deep .my-image {
       //   margin-right: 27rpx;
       // }
     }
// .equal-division {
//      margin-top: 22rpx;
//      ::v-deep .u-image {
//        margin-right: 27rpx;
//      }
//    }



</style>
