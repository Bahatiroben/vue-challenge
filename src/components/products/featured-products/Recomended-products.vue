<template>
    <div class="container">
      <div class="recommended-title-container">
        <h1>Products you might like</h1>
        <div class="navigator">
          <i class="fa fa-long-arrow-left" aria-hidden="true"></i>
          <i class="fa fa-long-arrow-right" aria-hidden="true"></i>
        </div>
      </div>
    <div class="image-container">
    <FeaturedProduct :key="product.id" v-for="product in products" :product="product"/>
  </div>
  </div>
</template>

<script>
import FeaturedProduct from "@/components/products/featured-products/Featured-product.vue"
export default {
  name: "RecomendedProducts",
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
    padding-bottom: 1rem;
    font-family: bodoni moda;
  }

  .recommended-title-container {
    display: flex;
    width: 85%;
    margin: auto;
    justify-content: space-between;
    align-items: center;
  }

  .navigator {
    width: 5%;
    display: flex;
    justify-content: space-between;
  }

  .fa-long-arrow-left {
    opacity: 0.2;
  }
  .container {
    background-color: #EDEAE6;
    padding-top: 5%;
    padding-bottom: 5%;
    margin-top: 5%;
    width: 100%;
  }
  .image-container {
    display: flex;
    width: 90%;
    margin: auto;
    justify-content: space-between;
    background-color: #EDEAE6;
    padding: 0rem!;
    flex-wrap: wrap;
    justify-content: space-between;
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

  @media screen and (max-width: 666px) {
    .image-container {
    width: 90%;
  }
}

</style>