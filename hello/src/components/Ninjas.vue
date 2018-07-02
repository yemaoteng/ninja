<template>
  <ul>
    <li v-for="ninja in ninjas" :key="ninja.id">
      {{ ninja.name }}
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      ninjas: [
        {name:'youmu',skill:'sword'},
        {name:'uuz',skill:'eat'},
        {name:'lingmeng',skill:'dream'}
      ]
    }
  },
}
</script>

<style scoped>
ul{
  margin: 5px;
}
ul::after{
  content: '';
  display: block;
  height: 0;
  clear: both;
}
li{
  list-style:none;
  width:200px;
  height:60px;
  border:1px solid grey;
  float: left;
  margin:10px;
}
</style>
