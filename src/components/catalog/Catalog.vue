<template>
  <h1>Catalog</h1>
  <div>
  <div class="row-1">
    <img src="../../assets/images/catalog/image1.jpeg"/>
  </div>
  <div class="row-2">
    <img src="../../assets/images/catalog/image2.jpeg"/>
    <img src="../../assets/images/catalog/image3.jpeg"/>
  </div>
</div>
</template>

<script>
import Category from "./Category.vue";
export default {
  name: "Catalog",
  components: {
    Category
  }
}
</script>

<style scoped>
  h1 {
    font-family: bodoni moda;
    font-size: 50px;
    font-weight: 700;
    line-height: 67px;
  }

  .row-1 img {
    width: 85%;
    margin: auto;
  }

  .row-2 {
    margin: auto;
    width: 85%;
    display: flex;
    justify-content: space-between;
  }

  .row-2 img {
    width: 49.5%;
  }


</style>
