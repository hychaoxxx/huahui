<template>
  <div class="hello">
    <img class="banner" src="../assets/Icon-App-60x60@3x.png"/>
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Huahui'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}
h1{
  font-size: 2rem;
  color: #fff;
  padding: 10px 0;
}
a {
  color: #42b983;
}
.banner{
  width: 20%;
}
.hello{
  padding: 60px 0;
  background: #6699FF;
  text-align: center;
}
</style>
