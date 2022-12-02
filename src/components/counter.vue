<template>
  <h1>Counter is here</h1>
  <h1>{{count}}</h1>
  <button v-on:click="count++">+</button>
  <button v-on:click="count--" >-</button>
<!--now we can execute the code in diff way by use of method-->
<button v-on:click="add">F+</button>
  <button v-on:click="reduce">F-</button>

<!--  now we can update name also using event objects-->
</template>
<script>
export default{
  data() {
    return {
      count: 0,
    }
  },
  //now by use of function in method we can inc our counter from here also without passing value in it
  //the better way to do this
  //now suppose we want to add it by 5 or any other number
  //we are having two ways one is simple just changing the value form 1 to any other number but for this we need to
  //change it everywhere so we can take an argument num and assign num a value in button componet so will get in better
  // way
  methods:{
    add(){
      this.count=this.count+1
    },
    reduce(){
      this.count=this.count-1
    }
  }
}
</script>