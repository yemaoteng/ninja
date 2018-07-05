<template>
  <div id="app">
    <img src="./assets/logo.png">
    <show-blogs></show-blogs>
  </div>
</template>

<script>
import showBlogsVue from './components/showBlogs.vue';


export default {
  name: 'app',
  components: {
    'show-blogs': showBlogsVue
  }
}
</script>

<style lang="scss" scoped>
#app {
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  margin-bottom: 60px;
}
</style>
