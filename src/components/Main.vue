<script>
import ProductCard from './partials/ProductCard.vue';
import products from '../components/data/product';

export default {

  data() {
    return {
      products
    }
  },
  components: {
    ProductCard
  },

}

</script>

<template>
  <main>
    <div class="container d-flex">

      <ProductCard v-for="product in products" :key="product.id" :productFrontImage="product.frontImage"
        :productBackImage="product.backImage" :productName="product.name" :productBrand="product.brand"
        :productPrice="product.price" />

    </div>
  </main>
</template>

<style lang="scss">
main {
  padding-top: 100px;

}
</style>