<template>
  <div id="nav" class="2">
    <div class="logo">
      <img src="../assets/logo.svg">
    </div>
    <ul>
      <li><router-link to="/">Home</router-link></li>
      <li><router-link to="/about">About</router-link></li>
      <li><router-link to="/contact">contact</router-link></li>
    </ul>
  </div>
  <router-view/>
</template>


<script>
export default {
  name:'Navbar',
}
</script>


<style>
  body {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  }
  ul{
    list-style: none;
    display: flex;
  }
  li{
    padding:10px;
  }
  #nav {
    padding: 30px;
  }

  #nav a {
    font-weight: bold;
    color: #2c3e50;
  }

  #nav a.router-link-exact-active {
    color: #42b983;
  }
  .logo img{
    width:50px;
  }
</style>