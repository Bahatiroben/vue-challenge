<template>
  <Highlight/>
  <Catalog/>
  <FeaturedProducts/>
  <TopBoughtProducts/>
  <RecomendedProducts/>
  <BestIdeas/>
</template>
<script>
  import Highlight from '@/components/Highlight.vue';
  import Catalog from '@/components/catalog/Catalog.vue';
  import FeaturedProducts from '@/components/products/featured-products/Featured-products.vue';
  import TopBoughtProducts from '@/components/products/featured-products/Top-bought-products.vue';
  import RecomendedProducts from '@/components/products/featured-products/Recomended-products.vue';
  import BestIdeas from '@/components/Best-ideas.vue';

  export default {
    name: 'Body',
    components: {
      Highlight,
      Catalog,
      FeaturedProducts,
      TopBoughtProducts,
      RecomendedProducts,
      BestIdeas
    }
  }
</script>

<style scoped>

</style>