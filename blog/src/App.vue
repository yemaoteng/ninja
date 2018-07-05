<template>
  <div id="app">
    <img src="./assets/logo.png">
    <add-blog></add-blog>
  </div>
</template>

<script>
import addBlogVue from './components/addBlog.vue';

export default {
  name: 'app',
  components: {
    'add-blog': addBlogVue
  }
}
</script>

<style lang="scss" scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
