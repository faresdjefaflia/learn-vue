<template>
  <div class="01">
    <Navbar />
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Footer from './components/Footer.vue';

export default {
  components:{
    Navbar,
    Footer,
  }
}
</script>


<style>
  /* FOR IMPORT CSS FILE */
  @import './assets/css/style.css';
  
  .txt p{
    text-align: left;
    width: 320px;
    margin: 0 auto;
    font-size: 18px;
    line-height: 26px;
  }

</style>