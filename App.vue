
<script>
  export default {
    data(){
      return {
        fullname:"Frank Aboagye",
        clsname : "theFullname",
        count: 0
      }
    },
    methods:{
      incre(){
        this.count++
      },
      decre(){
        this.count--
      }
    }
  }
</script>

<template>
  
  <h1 v-bind:class="clsname">
    Full name  = {{fullname}}
  </h1>
  
  <br>
  
  <button v-on:click="incre">
    Increment
  </button>
  
    <br>
  
  <button v-on:click="decre">
    Decrement
  </button>
  
    <br>
  
  <h2>
    The count is {{count}}
  </h2>
  
  

</template>


<style>
  
  .theFullname{
    color: blue;
  }

</style>
