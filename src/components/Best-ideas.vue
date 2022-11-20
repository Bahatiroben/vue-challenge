<template>
  <div class="container">
    <div class="best-ideas-image-container">
      <img src="../assets/images/best-ideas-sofa.jpeg"/>
    </div>
    <div class="best-ideas-container">
      <h1>The best ideas for sofas</h1>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Curabitur tempus urna at.</p>
        <div class="center">Show more
          <i class="fa fa-chevron-right" aria-hidden="true"></i>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BestIdeas",
}
</script>

<style scoped>
  h1 {
    font-family: bodoni moda;
    font-weight: 700;
    padding: 2rem;
    font-size: 57px;
    line-height: 67px;
  }

  .container {
    color: #FFFFFF;
    display: flex;
    justify-content: space-between;
  }

  .best-ideas-image-container {
    flex-basis: 60%;
  }

  .best-ideas-container {
    background-color: #1E1E1E;
    flex-basis: 40%;
    margin: 0px 0px 0.5% 2px;
  }

  .best-ideas-container p {
    font-size: 16px;
    padding: 2rem;
  }
  img {
    width: 100%;
  }

  button {
    height: 30px;
    border-radius: 40%;
  }

  .left {
    border: 1px solid white;
    width: 20px;
    border-right: none;
    border-radius: 40%;
  }

  .right {
    border: 1px solid white;
    border-left: none;
    width: 20px;
  }

  .center {
    background-color: transparent;
    color: #FFFFFF;
    border: 1PX solid rgba(255, 255, 255, 0.3);
    text-align: center;
    padding: 10px 20px;
    border-radius: 25px;
    width: 150px;
    font-weight: 700;
    margin-left: 2rem;
  }
</style>