<template>
  <div id="app">
    <app-header v-bind:title="title" v-on:fire="firechange"></app-header>
    <app-ninjas v-bind:ninjas="ninjas"></app-ninjas>
    <app-footer v-bind:title="title"></app-footer>
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
    'app-ninjas':Ninjas
  },
  data() {
    return {
      ninjas: [
        {name: 'Ryu', speciality: 'Vue Components', show: false},
        {name: 'Crystal', speciality: 'HTML Wizardry', show: false},
        {name: 'Hitoshi', speciality: 'Click Events', show: false},
      ],
      title:"This is a title"
    }
  },
  methods: {
    firechange:function() {
      this.title = 'change title from the top';
    }
  },

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
