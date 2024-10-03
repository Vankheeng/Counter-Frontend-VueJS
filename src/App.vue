<!-- <script setup>
  import {ref} from "vue";

  const count = ref(0);
</script> -->
  

<script>
  export default{
    data(){
      return {
        count: 0
      }
    },
    methods: {
      Add(){
        this.count = this.count + 1
      }, 
      Sub(){
        this.count = this.count - 1
      }
    }
    
  }
</script>


<template>
  <main>
    <div>
      <h4>
        The current count is ...
      </h4>
      <h1>{{ count }}</h1>
      <button @click="Sub()">-</button>
      <button @click="Add()">+</button>
    </div>
  </main>
</template>

<style scoped>
  main{
    background-color:  aliceblue;
    height: 100vh;
    width: 100vw;
    display: flex;
    align-items:  center;
    justify-content:  center;
  }
  div{
    text-align: center;
  }
</style>
