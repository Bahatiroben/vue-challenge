<template>
  <div class="container">
    <img :src="imageUrl"/>
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
  }

  img {
    width: 100%
  }
</style>