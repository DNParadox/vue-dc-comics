<template>
  <div id="app">
    <dcHeader />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import dcHeader from './components/dcHeader.vue'


export default {
  name: 'App',
  components: {
    // HelloWorld
    dcHeader,
  }
}
</script>

<style lang="scss">
@import './style/common';

</style>
