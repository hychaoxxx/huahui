<template>
  <div id="app">
    <audio></audio>
    <hello></hello>
    <list></list>
  </div>
</template>

<script>
import Hello from './components/Hello'
import List from './components/List'
export default {
  name: 'app',
  components: {
    Hello,
    List
  }
}
</script>

<style>
*{
  margin:0;
  padding: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
