<template>
    <div class="card">
      <h3>{{name}}:</h3>
      <h3>{{age}} year</h3>
    </div>
</template>

<script>
export default {
  name:'Props',
  props:{
    name:String,
    age:Number,
  }
}
</script>

<style>
  .card{
    display: flex;
    border: solid 1px #2c3e50;
    border-radius:6px;
    padding:8px;
  }
  .card h3{
    font-size: 16px;
    margin: 0;
  }
</style>