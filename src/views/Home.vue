<template>
  <main>
    <h1> HELLO FROM "HOME"</h1>
    <Hometxt />
    <p v-bind:class="listClass.name">{{myName() + " " + nameHello }}</p>
  </main>
</template>


<script>
import Hometxt from '../components/home/Home-txt';

//JS
let prompHello;
if(localStorage.theName){
  prompHello = localStorage.theName
} else{
  prompHello = prompt("ENTER YOUR NAME")
  localStorage.setItem("theName", prompHello);
}
//

export default {
  components:{
    Hometxt,
  },
  data() {
    return {
      nameHello:prompHello,
      listClass: {
        name:'name',
      }
    }
  },
  methods: {
    myName(){
      return 'Hello'
    }
  },
}
</script>

<style>
  .name{
    font-size:24px;
    font-weight: bold;
    color: blue;
  }
</style>