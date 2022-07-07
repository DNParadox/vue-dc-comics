<template>
  <div id="app">
    <dcHeader />

     <main>
      <dcJumbotron />
      <sectionContent />
      <sectionProduct />
    </main>



    <dcFooter />
  </div>
</template>

<script>
import dcHeader from './components/dcHeader.vue'
import sectionContent from "./components/sectionContent.vue";
import sectionProduct from "./components/sectionProduct.vue"
import dcFooter from "./components/dcFooter.vue"
import dcJumbotron from './components/dcJumbotron.vue';

export default {
  name: 'App',
  components: {
    dcHeader,
    dcJumbotron,
    sectionContent,
    sectionProduct,
    dcFooter,

  }
}
</script>

<style lang="scss">
@import './style/common';


</style>
