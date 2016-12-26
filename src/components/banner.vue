<template>
  <div class="banner">
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <div id="example-1">
      <button v-on:click="counter += 1">Add 1</button>
      <p>The button above has been clicked {{ counter }} times.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'banner',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      counter:0
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

</style>
