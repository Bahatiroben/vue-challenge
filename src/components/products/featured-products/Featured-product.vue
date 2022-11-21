<template>
  <div :style="style" class="container">
    <div class="overlay-container">
    <div class="overlay">
      <h3>{{product.title}}</h3>
      <img class="logo mobile-hidden" :src="product.logo"/>
      <div class="price mobile-hidden">from ${{product.price}}/meter</div>
      <div class="circles">
        <div class="circle red"></div>
        <div class="circle grey"></div>
        <div class="circle green"></div>
        <div class="circle black"></div>
        <div>+20</div>
      </div>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FeaturedProduct',
  props: {
    product: Object
  },
  computed: {
    style() {
      return `background-image: url("${this.product.imageUrl}")`
    }
  }
}
</script>

<style scoped>
  .container {
    width: 100%;
    background-repeat: no-repeat;
    background-size: 100%;
    margin: 0px;
    padding: 0px;
    flex-basis: 24%;
  }

  h3 {
    font-weight: 700;
    margin-top: 15px;
  }

  .price {
    margin-bottom: 15px;
  }

  .logo {
    opacity: 1;
    width: 70px;
    padding: 10px;
  }


  .overlay-container:hover {
    opacity: 1
  }

  .overlay-container {
    background-color: transparent;
    width: 100%;
    font-size: 14px;
    height: 50vh;
    padding: 0px;
    margin: 0px;
    display: flex;
    flex-direction: column;
    justify-content: end;
    opacity: 0;
  }

  .overlay {
    background-color: white;
    width: 100%;
    font-size: 14px;
    min-height: 36%;
  }

  .overlay:hover {
    opacity: 1
  }

  .overlay-hidden {
    opacity: 0;
  }

  .circles {
    display: flex;
    justify-content: space-between;
    width: 80%;
    margin: auto;
    font-size: 14px;
    padding-bottom: 10px;
  }

  .circle {
    height: 20px;
    width: 20px;
    border-radius: 50%;
  }

  .red {
    background-color: maroon;
  }

  .grey {
    background-color: grey;
  }

  .green {
    background-color: rgb(13, 66, 13);
  }

  .black {
    background-color: black;
  }

  @media screen and (max-width: 666px) {
    .container {
    flex-basis: 100%;
  }

  .overlay-container {
    height: 60vh;
    opacity: 1;
  }
  }
</style>