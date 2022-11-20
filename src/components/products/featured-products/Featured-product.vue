<template>
  <div class="container">
    <img class="main-image" :src="imageUrl"/>
    <div class="overlay-container">
    <div class="overlay">
      <h3>Lorem ipsum dolor sit</h3>
      <img class="logo" src="../../../assets/logos/brignoli-grey.svg"/>
      <div class="price">from $12/meter</div>
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
  props: {
    imageUrl: String
  }
}
</script>

<style scoped>
  .container {
    width: 100%;
    display: block;
    position: relative;
  }

  h3 {
    font-weight: 700;
    margin-top: 15px;
  }

  .main-image {
    width: 100%
  }

  .price {
    margin-bottom: 15px;
  }

  .logo {
    opacity: 1;
    width: 70px;
    padding: 10px;
  }

  .overlay-container {
    position: absolute;
    z-index: 1;
    min-height: 100%;
    width: 100%;
    top: 0;
    background-color: transparent;
    opacity: 0;
  }

  .overlay-container:hover {
    opacity: 1
  }

  .overlay {
    background-color: white;
    width: 100%;
    font-size: 14px;
    position: absolute;
    top: 62%;
    min-height: 34%;
  }

  .overlay:hover {
    opacity: 1;
  }

  .overlay-hidden {

  }

  .circles {
    display: flex;
    justify-content: space-between;
    width: 80%;
    margin: auto;
    font-size: 14px;
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
</style>