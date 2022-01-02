<template>
  <header id="nav">
    <div class="logo">
      <img src="../assets/logo.svg">
    </div>
    <ul>
      <li><router-link to="/">HOME</router-link></li>
      <li><router-link to="/about">ABOUT</router-link></li>
      <li><router-link to="/contact">CONTACT</router-link></li>
    </ul>
  </header>
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
    border-bottom: solid 1px #2c3e50;
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
    text-decoration: none;
  }

  #nav a.router-link-exact-active {
    color: #42b983;
  }
  .logo img{
    width:50px;
  }
</style>