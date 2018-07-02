<template>
  <div id="app">
    <app-header></app-header>
    <ninjas></ninjas>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Ninjas from './components/Ninjas.vue';

export default {
  name: 'app',
  components: {
    'app-header':Header,
    'app-footer':Footer,
    'ninjas':Ninjas
  }
}
</script>

<style>
* {
  box-sizing: border-box;
}
html,
body{
  margin:0;
  padding:0;
}
</style>
