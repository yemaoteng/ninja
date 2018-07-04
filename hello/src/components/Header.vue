<template>
  <div class="header">
    <h1>This is Header</h1>
    <p>{{htitle}}</p>
    <button @click="changetitle">Ha?</button><br/>
    <button @click="usebus">Use Bus</button>
    <p>bustext: {{bustext}}</p>
  </div>
</template>

<script>
import {bus} from '../main';

export default {
  props:{
    title:{
      type:String
    }
  },
  data(){
    return {
      bustext:"emptybustext"
    }
  },
  methods: {
    changetitle:function() {
      //this.title='vue wizard';
      this.$emit('fire','wizard')
    },
    usebus:function(){
      this.bustext = "bus start";
      bus.$emit('busfire','bus start');
    }
  },
  computed:{
    htitle:function(){
      return this.title
    }
  }
}

</script>

<style scope>
.header {
  background-color: green;
}
h1{
  background-color: lightgreen;
  color:#222;
  text-align: center;
  line-height: 60px;
  margin:0 0 30px 0;
}
</style>