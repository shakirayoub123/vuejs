<template>
  <br>
<h1>EVENTS</h1>
  <form v-on:submit.prevent="submitForm">
    <input type="text" v-on:input="setName($event,'jazz')" v-on:keyup.enter="confirmedInput">
 <p>Name:{{confirmedName}}</p>
  <button>sign up</button>
  </form>

</template>
<script>
export  default {
  data(){


    return{
     name:'',
      confirmedName:'',

    }
  },
  methods:{
    //by using this our data wont be removed after clicking on submit form so we use event.preventDefault()
    //and data will be there as we were using this in dom before but in vue its quite easy to use now
    confirmedInput(){
   this.confirmedName=this.name;
    },

    submitForm(){
      // event.preventDefault();
    alert('data submited');
    },
    setName(event){
      this.name=event.target.value
    }
  }


}


</script>