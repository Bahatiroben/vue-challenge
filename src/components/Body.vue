<template>
  <Highlight/>
  <Catalog/>
</template>
<script>
  import Highlight from '@/components/Highlight.vue';
  import Catalog from '@/components/catalog/Catalog.vue';
  export default {
    name: 'Body',
    components: {
      Highlight,
      Catalog
    }
  }
</script>

<style scoped>

</style>