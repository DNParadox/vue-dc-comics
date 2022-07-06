<template>
  <div id="app">
    <dcHeader />

   <main>
     <sectionContent />
     <sectionProduct />
   </main>
  
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import dcHeader from './components/dcHeader.vue'
import sectionContent from "./components/sectionContent.vue";
import sectionProduct from "./components/sectionProduct.vue"

export default {
  name: 'App',
  components: {
    dcHeader,
    sectionContent,
    sectionProduct,
  }
}
</script>

<style lang="scss">
@import './style/common';

</style>
