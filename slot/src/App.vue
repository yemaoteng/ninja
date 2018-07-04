<template>
  <div>
    <h1>This is App.vue</h1>
    <app-son></app-son>
  </div>
</template>

<script>
import son from "./components/son.vue";

export default {
  components: {
    "app-son": son
  }
};
</script>

<style>
</style>
