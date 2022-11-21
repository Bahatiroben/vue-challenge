<template>
  <div class="container">
  <h1 class="catalog-title">Catalog</h1>
  <div>
  <div class="row-1 img-container">
    <div class="image image-1">
    <div class="catalog-highlight">
      <h1 class="highlight-element">Tessuri</h1>
      <div class="separator"/>
      <p class="highlight-element">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis.</p>
    </div>
    </div>

    <div class="image image-2">
    <div class="catalog-highlight">
      <h1 class="highlight-element">Tessuri</h1>
      <div class="separator"/>
      <p class="highlight-element">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    </div>
    </div>

    <div class="image image-3">
    <div class="catalog-highlight">
      <h1 class="highlight-element">Tessuri</h1>
      <div class="separator"/>
      <p class="highlight-element">Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
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


  .row-1 img {
    width: 100%;
  }


  .img-container {
    display: flex;
    flex-wrap: wrap;
  }

  .image {
    display: flex;
    color: #FFFFFF;
    background-repeat: no-repeat;
    margin: 2px;
  }

  .image-1 {
    background-image: url("../../assets/images/catalog/image1.jpeg");
    height: 450px;
    flex-basis: 99%;
    background-size: cover;
  }

  .image-2 {
    background-image: url("../../assets/images/catalog/image2.jpeg");
    height: 450px;
    flex-basis: 49.5%;
    background-size: cover;
  }

  .image-3 {
    background-image: url("../../assets/images/catalog/image3.jpeg");
    height: 450px;
    flex-basis: 49.2%;
    background-size: cover;
  }

  .catalog-highlight {
    width: 40%;
    margin: auto;
  }

  .highlight-element {
    margin: 20px;
  }


  @media screen and (max-width: 666px) {
    .catalog-title {
    width: 90%;
    margin: 0px auto 1rem auto;
    font-size: 40px;
    line-height: 50px;  
  }

  .row-1 {
    width: 90%;
  }

  .container {
    margin-top: 0px;
  }

  .image {
    flex-basis: 100%;
  }

  .catalog-highlight {
    width: 80%;
  }

  .row-1 {
    width: 90%;
  }


  }

</style>
