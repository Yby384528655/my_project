<template>
  <div id="app">
    <img src="./assets/logo.png">
    <banner2></banner2>
    <hello></hello>
    <h1>{{msg}}</h1>
    <input type="text" v-model='msg'>
  </div>
</template>

<script>

import Banner2 from './components/banner2'
import Hello from './components/Hello'
export default {
  name: 'app',
  components: {
    Banner2,
    Hello
  },
  data(){
    return{
      msg:"hello"
    }
  }
}
</script>

<style>
*{margin:0;padding:0;}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
