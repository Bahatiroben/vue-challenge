<template>
  <div class="container">
    <div class="container-top-products">
      <h1 class="top-bought-title">Top bought products</h1>
      <div class="top-bought-description">
        <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Curabitur tempus urna at turpis condimentum lobortis. Ut commodo efficitur neque. Ut diam quam, semper iaculis condimentum ac, vestibulum eu nisl.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Curabitur tempus urna at turpis
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis. Class aptent taciti sociosqu ad litora torquent per conubia nostr
      </p>
      </div>
    </div>
    <div class="image-container">
      <img src="../../../assets/images/liked-products/image1.jpeg"/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TopBoughtProduct',
  components: {
  }
}
</script>

<style scoped>
  

  h1 {
    font-family: bodoni moda;
    margin-bottom: 20px;
  }
  .container-top-products {
    flex-basis: 40%;
    margin: auto;
  }

  .top-bought-description p {
    padding-bottom: 20px;
  }

  .container {
    display: flex;
    margin: auto;
    justify-content: space-between;
    padding: 5rem 5rem 0rem 5rem;
    flex-wrap: wrap;
    align-items: center;
  }

  img {
    width: 80%;
    margin: auto;
  }

  .image-container {
    flex-basis: 60%;
  }

  @media screen and (max-width: 666px) {
    .container {
    width: 90%;
    padding: 0px;
    margin: auto;
  }
  .container-top-products {
    width: 90%;
  }

  .image-container {
    flex-basis: 100%;
  }

  .container-top-products {
    flex-basis: 100%;
  }
}
</style>