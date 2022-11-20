<template>
  <div class="container">
  <h1 class="catalog-title">Catalog</h1>
  <div>
  <div class="row-1 img-container">
    <img src="../../assets/images/catalog/image1.jpeg"/>
    <div class="catalog-highlight">
      <h1>Tessuri</h1>
      <div class="separator"/>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis.</p>
    </div>
  </div>
  <div class="row-2">
    <div class="img-container container-1">
      <img src="../../assets/images/catalog/image2.jpeg"/>
      <div class="catalog-highlight">
        <h1>Category</h1>
        <div class="separator"/>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
      </div>
    </div>
    <div class="img-container container-1">
      <img src="../../assets/images/catalog/image3.jpeg"/>
      <div class="catalog-highlight">
        <h1>Category</h1>
        <div class="separator"/>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
      </div>
    </div>
  </div>
</div>
</div>
</template>

<script>
export default {
  name: "Catalog",
}
</script>

<style scoped>
  h1 {
    font-family: bodoni moda;
    font-size: 50px;
    font-weight: 700;
    line-height: 67px;
  }

  .separator {
    height: 1px;
    width: 40px;
    margin: 20px auto;
    background-color: #FFFFFF;
  }

  .catalog-title {
    width: 85%;
    display: flex;
    margin: 2rem auto;  
  }

  .container {
    margin-top: 10vh;
  }

  .row-1 {
    width: 85%;
    margin: auto;
  }

  .img-container {
    position: relative;
  }

  .row-1 img {
    width: 100%;
  }

  .row-2 {
    margin: auto;
    width: 85%;
    display: flex;
    justify-content: space-between;
  }

  img {
    width: 100%;
  }

  .catalog-highlight {
    position: absolute;
    top: 15vh;
    left: 30%;
    z-index: 1;
    width: 40%;
    margin-left: auto;
    margin-right: auto;
    color: #FFFFFF;
  }


  .container-1 {
    width: 49.5%;
  }

</style>
