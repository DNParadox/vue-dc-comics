<template>
  <div class="container">
    <div class="test">
         <singleCardComponent v-for="(element,index) in products" :key="index" :cardDetails="element"/>
    </div>
    
  </div>
</template>

<script>
import dcComicsJson from '../assets/dc-comics.json';
import singleCardComponent from '../components/CardComponent.vue'

export default {
    name: 'sectionContent',
    components: 
        {
        singleCardComponent 
        },

    data() {
        return {
            products: dcComicsJson,
        };
    }
}
</script>

<style scoped lang="scss">

section {
    height: 350px;
}
div {
    color: white;
}

.test{
    display: flex;
    flex-wrap: wrap;
    
}
</style>