<template>
  <footer>
    <p>This is footer{{foottitle}}</p>
    <br/>
    <p>bustext: {{bustext}}</p>
  </footer>
</template>

<script>
import {bus} from '../main';

export default {
  props:{
    title:{
      type:String
    }
  },
  data() {
    return {
      bustext: "still empty"
    }
  },
  computed:{
    foottitle:function(){
      return this.title;
    }
  },
  created() {
    bus.$on('busfire',(data)=>{
      this.bustext = data;
    })
  },
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
