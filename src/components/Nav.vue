<template>
  <div class="header-container">
    <div class="main-logo">
      <img src="../assets/logos/brignoli.svg"/>
    </div>
    <div class="nav-options-section">
      <div class="nav-catalog">CATALOG</div>
      <div class="nav-options">
        <NavList :options="options" />
      </div>
    </div>
  </div>
</template>

<script>
  import NavList from '@/components/NavList';
  export default {
    name: 'Nav',
    components: {
      NavList
    },

    data: () => ({options: ["SOLUTIONS", "NEWS", "PROJEsCTS", "SOLUTIONS", "NEWS", "PROJECTS"]}),
    // methods: {
    //   created() {
    //     this.options = ["SOLUTIONS", "NEWS", "PROJECTS", "SOLUTIONS", "NEWS", "PROJECTS"]
    //   },
    // }
  }
</script>

<style scoped>
  @import url('https://fonts.cdnfonts.com/css/montserrat');
  .header-container {
    width: 100%;
    background-color: #A3846B;
    font-family: 'Montserrat', sans-serif;
    font-size: 20px;
    color: #FFFFFF;
    display: flex;
    justify-content: space-between;
  }

  .main-logo {
    padding: 10px 80px 19px 80px;
    height: 72px;
  }

  .nav-options-section {
    padding: 19px 80px;
    height: 72px;
    width: 40%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .nav-options {
    width: 80%;
  }

  .nav-catalog {
    font-weight: 700;
    padding-right: 12.5px;
    word-break: normal;
    white-space:pre
  }

  .header-login img {
    position: relative;
    top: 2.5px;
  }

</style>