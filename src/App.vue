<template>

 
  
  <Test msg="Hola!!!!"/>
  <User/>
  
</template>

<script>

import Test from './components/Test.vue';
import User from './components/User.vue';


export default {
  name: 'App',
  components: {
    Test,
    User
   
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}




</style>
