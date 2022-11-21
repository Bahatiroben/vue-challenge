<template>
  <div class="header-container">
    <div class="main-logo">
      <div class="logo-container"></div>
    </div>
    <div class="header-login">
      <div class="login">
        <img class="login-icon" src="../assets/icons/person.icon.svg"/>
        <span class="login-caption">LOG IN</span>
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
    display: flex;
    justify-content: center;
    align-items: center;
    padding-left: 5rem;
  }

  .logo-container {
    background-image: url("../assets/logos/martineli-logo.svg");
    min-width: 250px;
    height: 70px;
    background-repeat: no-repeat;
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

  @media screen and (max-width: 500px) {
    .main-logo {
    display: flex;
    justify-content: center;
    align-items: center;
    padding-left: 5rem;
  }

  .logo-container {
    background-image: url("../assets/logos/group.logo.svg");
    min-width: 50px;
    height: 70px;
    background-repeat: no-repeat;
  }

  .main-logo {
    display: flex;
    justify-content: center;
    align-items: center;
    padding-left: 2rem;
  }

  .header-login {
    padding: 15px 20px;
    width: 245px;
    height: 72px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }

  .login-icon {
    padding-right: 2rem;
  }

  .login-caption {
    display: none;
  }

  }

</style>