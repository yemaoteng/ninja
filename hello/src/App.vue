<template>
  <div id="app">
    <p>Here is miemie</p>
    <miemie mmm="qqqqqqqq"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import miemie from './components/miemie.vue';

export default {
  name: 'app',
  components: {
    HelloWorld,
    miemie
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h1{
  color:yellow;
}
</style>
