<template>
  <div>
    <app-son>
      <p slot="foot-slot">This is p to son</p>
      <h2 slot="head-slot">This is h2 to son</h2>
      
    </app-son>
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
