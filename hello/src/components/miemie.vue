<template>
  <div class="miemie">
    <h1>This is miemie h1 title</h1>
    <mumu></mumu>
  </div>
</template>

<script>
import mumu from './mumu.vue'

export default {
  name: 'miemie',
  props: {
    mmm: String
  },
  components:{
    mumu
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1{
  color:red;
}
</style>
