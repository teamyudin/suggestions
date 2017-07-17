<template>
  <el-menu theme="dark" :default-active="activeIndex" mode="horizontal" :router=true>
    <el-menu-item index="/">Home</el-menu-item>
    <el-menu-item index="about">About</el-menu-item>
  </el-menu>
</template>

<script>
  export default {
    data () {
      return {
        activeIndex: '/'
      }
    }
  }
</script>

<style scoped>

</style>
