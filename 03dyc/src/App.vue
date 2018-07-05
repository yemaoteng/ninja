<template>
  <div id="app">
    <button @click="formtype='form1'">腾讯</button>
    <button @click="formtype='form2'">阿里</button>
    <keep-alive>
      <component v-bind:is="formtype"></component>    
    </keep-alive>
  </div>
</template>

<script>
import form1 from './components/form1.vue';
import form2 from './components/form2.vue';

export default {
  name: 'app',
  components: {
    form1:form1,
    form2:form2
  },
  data() {
    return {
      formtype: 'form1'
    }
  },
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
</style>
