<script>
import ProductCard from './partials/ProductCard.vue';
import products from './data/product.json';
export default {
  data() {
    return {
      products
    }
  },
  components: {
    ProductCard
  },
  mounted() {
    console.log(this.products.products);
  }
}
</script>

<template>
  <main>
    <div class="container d-flex">

      <ProductCard v-for="(product) in products.products" :key="product.id" :FrontImage="`/img/${product.frontImage}`"
        :BackImage="`/img/${product.backImage}`" :Name="product.name" :Brand="product.brand"
        :FullPrice="product.price" />

    </div>

  </main>
</template>

<style lang="scss">
main {
  padding-top: 100px;

}
</style>