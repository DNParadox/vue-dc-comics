<template>
          <figure class="card-content">
            <img class="cardimage" :src="cardDetails.thumb" alt="cardDetails.series">
            <figcaption class="card-title">{{ cardDetails.series}}</figcaption>
         </figure>
</template>

<script>
export default {
    name: "singleCardComponent",
    props: {
        cardDetails: Object
    }
}
</script>



<style scoped lang="scss">
.card-content{
    padding-inline: 0.3rem;
    width: calc((100% / 6) - 0.6rem );
    padding-block: 1.2rem;
}
.card-title {
    font-size: 0.7rem;
}

.cardimage {
    width: 100%;
    object-fit: cover;
    object-position: top;
    aspect-ratio: 1 / 1;
}
</style>

