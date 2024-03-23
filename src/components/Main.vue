<script>
import ProductCard from './partials/ProductCard.vue';
import products from '../components/data/product.json';

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

      <ProductCard v-for="(product) in products.products" :key="product.id"
        :FrontImage="`src/assets/img/${product.frontImage}`" :BackImage="`src/assets/img/${product.BackImage}`"
        :Name="product.name" :Brand="product.brand" :FullPrice="product.price" />

    </div>
  </main>
</template>

<style lang="scss">
main {
  padding-top: 100px;

}
</style>