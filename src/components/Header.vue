<template>
  <div class="header-container">
    <div class="main-logo">
      <img src="../assets/logos/martineli-logo.svg"/>
    </div>
    <div class="header-login">
      <div class="login">
        <img src="../assets/icons/person.icon.svg"/>
        <span>LOG IN</span>
      </div>
      <div>
        <img src="../assets/icons/menu-toggle.svg"/>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Header',
    components: {
      
    },
    setup() {
      
    },
  }
</script>

<style scoped>
  @import url('https://fonts.cdnfonts.com/css/montserrat');
  .header-container {
    width: 100%;
    background-color: #000000;
    font-family: 'Montserrat', sans-serif;
    color: #FFFFFF;
    display: flex;
    justify-content: space-between;
    overflow: hidden;
    word-break:break-all
  }

  .main-logo {
    padding: 19px 80px;
    width: 245px;
    height: 72px;
  }

  .header-login {
    padding: 19px 80px;
    width: 245px;
    height: 72px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .header-login img {
    position: relative;
    top: 2.5px;
  }

</style>