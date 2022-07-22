<script setup>
import { ref ,watch } from 'vue'

const props = defineProps({
  arr: Array
})
console.log("props:",props)
//
watch(props.arr,(arr)=>{
  console.log("直接取值,arr改变：",arr)
})
watch(()=>props.arr,(arr)=>{
  console.log("函数返回值,arr改变：",arr)
})
</script>

<script>
  export default {
    props:{
      arr:Array
    },
    watch: {
      arr(value) {
        console.log("option选项的watch：",value)
      }
    }
  }
</script>

<template>
  arr --> {{arr}}
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
