<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue'
import {ref} from 'vue'
let arr = ref([])

setTimeout(()=>{
  console.log('直接赋值')
  arr.value = [1,2,3]
},1500)

// 1.这里是第二次改变值，先注释，先看上面的
// 2. 注释上面的，解开下面注释，两个分别对比
// 3. 最后两段解开注释同时运行观察对比


setTimeout(()=>{
   console.log('使用push')
  arr.value.push(1)
 
},2500)

</script>

<template>
  <HelloWorld :arr = "arr"/>
</template>

<style>

</style>
