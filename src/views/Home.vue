<template>
  <main>
    <h1> HELLO FROM "HOME"</h1>
    <Hometxt />
    <p v-bind:class="listClass.name">{{myName() + " " + nameHello }}</p>
    <button v-bind:class="listClass.margin" v-on:click="getConsole()">Print Name</button>
    <div>
      <label v-bind:class="listClass.margin">Edit name :</label>
      <input v-bind:class="listClass.margin" type="text" placeholder="edit" v-model="nameHello">
    </div>
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
        margin:'mrgn'
      }
    }
  },
  methods: {
    myName(){
      return 'Hello'
    },
    getConsole(){
      console.log(prompHello)
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
  .mrgn{
    margin: 10px;
  }
</style>