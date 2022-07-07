<template>
  <section>
    <div class="jumbotron">
        <img src="../assets/img/jumbotron.jpg" alt="Teen Titans">     
    </div>
  </section>
</template>

<script>

export default {
    name: 'dcJumbotron',
}
</script>

<style scoped lang="scss">
@import '../style/variables.scss';

section {
    display: flex;
    height: 330px; 
    .jumbotron {
      color: white;
      width: 100%;
      height: 50%;  
}
  img {
      width: 100%;
      height: 300px;
      object-fit: cover;
      object-position: top;
      }
}

</style>