<template>
  <section>
    <div class="container">


        <div v-for="product,index in productList" :key="index" class="card">
          <img :src="product.img" alt="digital comics">
          <div class="cardtext">{{product.text }}</div>
        </div>


    </div>
  </section>
</template>

<script>
export default {
  name: 'sectionContent',
  data() {
    return {
      productList: [
        {
          img: require('../assets/img/buy-comics-digital-comics.png'),
          text: 'DIGITAL COMICS'
        },
        {
          img: require('../assets/img/buy-comics-merchandise.png'),
          text: 'DC MERCHANDISE'
        },
          {
          img: require('../assets/img/buy-comics-subscriptions.png'),
          text: 'SUBSCRIPTION'
        },
        {
          img: require('../assets/img/buy-comics-shop-locator.png'),
          text: 'COMIC SHOP LOCATOR'
        },
         {
          img: require('../assets/img/buy-dc-power-visa.svg'),
          text: 'DC POWER VISA'
        },
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import '../style/variables.scss';

.container {
  width: 65%;
  height: 100%;
}

section {
  background-color: $brand_main_color;
}

.cardtext {
  color: $brand_secondary_color;
}
</style>