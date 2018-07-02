<template>
  <footer>
    This is footer{{foottitle}}
  </footer>
</template>

<script>
export default {
  props:{
    title:{
      type:String
    }
  },
  computed:{
    foottitle:function(){
      return this.title;
    }
  }
}
</script>

<style scoped>
footer {
  background:#222;
  color:lightgreen;
  text-align: center;
  line-height: 40px;
}
</style>
