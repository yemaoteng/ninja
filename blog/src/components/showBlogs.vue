<template>
<div id="show-blogs">
    <h1>BLOGS</h1>
    <div v-for="blog in blogs" :key="blog.id">
        <h2>{{blog.title}}</h2>
        <article>{{blog.body}}</article>
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            blogs:[]
        }
    },
    methods: {
       
    },
    created() {
        this.$http.get('http://jsonplaceholder.typicode.com/posts').then(function(data){
            this.blogs = data.body.slice(0,10);
        })
    },
}
</script>

<style lang="scss" scoped>

</style>
