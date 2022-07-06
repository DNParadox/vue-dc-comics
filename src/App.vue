<template>
  <div id="app">
    <dcHeader />

     <main>
      <sectionContent />
      <sectionProduct />
    </main>




  </div>
</template>

<script>
import dcHeader from './components/dcHeader.vue'
import sectionContent from "./components/sectionContent.vue";
import sectionProduct from "./components/sectionProduct.vue"
import footer from 

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
