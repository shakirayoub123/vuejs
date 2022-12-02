<template>
<h1 v-on:mousemove="getConsole()">Home</h1>
  <button v-on:click="getData('Button 1 clicked')">Click me</button>
  <button v-on:dblclick="getData('Button 1 clicked')">Click me</button>
  <h2>{{count}}</h2>
<!--  using events for making count-->
  <button v-on:click="count--">dec</button>
  <button v-on:click="count++">inc</button>
</template>

<script>
export  default {
        name:"Home",
  data(){
          return{
            count:0
          }
  },
  methods:{
          getData(data)
          {
            alert(data)
          },
    getConsole()
    {
      console.log("danger")
    }
  }
}
</script>
<style>

h1{
  color:green;


}
</style>