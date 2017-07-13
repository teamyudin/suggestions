<template>
  <div id="app">
    <div id="surface">
      <div id="header">
        <Navbar />
      </div>
      <div id="content">
        <transition name="fade">
          <router-view></router-view>
        </transition>
      </div>
    </div>
  </div>
</template>

<script>

import Navbar from '@/components/navbar'

export default {
  name: 'app',
  components: {
    Navbar
  }
}
</script>

<style>
  body{
    margin: 0;
    background-color: rgb(0, 121, 191)
  }

  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  .fade-enter-active, .fade-leave-active {
    transition-property: opacity;
    transition-duration: .25s;
  }

  .fade-enter-active {
    transition-delay: .25s;
  }

  .fade-enter, .fade-leave-active {
    opacity: 0
  }

</style>
