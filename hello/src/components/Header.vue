<template>
  <div>
    <h1>This is Header</h1>
    <p>{{htitle}}</p>
    <button @click="changetitle">Ha?</button>
  </div>
</template>

<script>

export default {
  props:{
    title:{
      type:String
    }
  },
  data(){
    return {}
  },
  methods: {
    changetitle:function() {
      //this.title='vue wizard';
      this.$emit('fire','wizard')
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
h1{
  background-color: lightgreen;
  color:#222;
  text-align: center;
  line-height: 60px;
  margin:0 0 30px 0;
}
</style>