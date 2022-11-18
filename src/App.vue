<template>
  <Header/>
  <Nav/>
  <Body/>
  <router-view/>
</template>

<script>
  import Header from '@/components/Header.vue';
  import Nav from '@/components/Nav.vue';
  import Body from '@/components/Body.vue';
  export default {
    name: 'App',
    components: {
      Header,
      Nav,
      Body
    }
  }
</script>


<style>
* {
    margin: 0;
    padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

/* body {
  background-color: #000000;
} */

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
