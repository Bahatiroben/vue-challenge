<template>
  <div class="container">
    <h1>Featured products</h1>
    <div class="image-container">
    <div class="feature-product-container" :key="product.id" v-for="product in products">
      <FeaturedProduct :product="product"/>
    </div>
  </div>
  </div>
</template>

<script>
  import FeaturedProduct from '@/components/products/featured-products/Featured-product.vue';
  export default {
    components: {
      FeaturedProduct
    },
    data: () => ({products: [
      {
        title: 'Lorem ipsum dolor sit',
        id: 1,
        price: 12,
        imageUrl: require("../../../assets/images/featured-products/image1.jpeg"),
        logo: require("../../../assets/logos/brignoli-grey.svg") 
      },
      {
        title: 'Lorem ipsum dolor sit',
        id: 2,
        price: 12,
        imageUrl: require("../../../assets/images/featured-products/image2.jpeg"),
        logo: require("../../../assets/logos/brignoli-grey.svg") 
      },
      {
        title: 'Lorem ipsum dolor sit',
        id: 3,
        price: 12,
        imageUrl: require("../../../assets/images/featured-products/image3.jpeg"),
        logo: require("../../../assets/logos/brignoli-grey.svg") 
      },
      {
        title: 'Lorem ipsum dolor sit',
        id: 4,
        price: 12,
        imageUrl: require("../../../assets/images/featured-products/image4.jpeg"),
        logo: require("../../../assets/logos/brignoli-grey.svg") 
      }
    ]})
  }
</script>

<style scoped>
  
  h1 {
    display: flex;
    width: 85%;
    margin: auto;
    padding-bottom: 1rem;
    font-family: bodoni moda;
  }
  .container {
    background-color: #EDEAE6;
    padding-top: 5%;
    padding-bottom: 5%;
    margin-top: 5%;
  }
  .image-container {
    display: flex;
    width: 85%;
    margin: auto;
    justify-content: space-between;
    background-color: #EDEAE6;
    padding: 0rem!;
  }
  .feature-product-container:nth-child(2) {
    padding-right: 20px;
  }
  .feature-product-container:nth-child(1) {
    padding-right: 20px;
  }
  .feature-product-container:nth-child(4) {
    padding-left: 20px;
  }
</style>