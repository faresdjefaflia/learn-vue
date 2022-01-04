<template>
  <h1> HELLO FROM "ABOUT" </h1>
  <Aboutetxt />
  <div class="contr">
    <h1>Contributors</h1>
      <div class="all-cards">
        <Props name="fares1" age="23"/>
        <Props name="fares2" age="23"/>
        <Props name="fares3" age="23"/>
        <Props name="fares4" age="23"/>
        <Props name="fares5" age="23"/>
      </div>
      <div class="date">
        <p>{{day}} {{date}}</p>
        
      </div>
  </div>
</template>


<script>
import Aboutetxt from '../components/about/About-txt';
import Props from '../components/about/Props.vue';
export default {
  components:{
    Aboutetxt,
    Props,
  },
  data() {
    return {
      day:'M',
      date:'jan  3 2022',
    }
  },
}
</script>

<style>
  .contr{
    text-align: left;
    width:60%;
    margin: 30px auto;
  }
  .all-cards{
    display: flex;
    justify-content: space-around;
  }
  .contr h1{
    font-size:24px;
  }
</style>