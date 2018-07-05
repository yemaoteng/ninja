<template>
<div id="add-blog">
    <h1>Add Blog Page</h1>
    <h3>Blog title</h3>
    <input type="text" v-model="blog.title"/>
    <h3>Blog content</h3>
    <textarea v-model="blog.content"/>
    <input type="checkbox" value="ninja" v-model="blog.categories">
    <span>ninja</span>
    <input type="checkbox" value="wizard" v-model="blog.categories">
    <span>wizard</span>
    <input type="checkbox" value="scientist" v-model="blog.categories">
    <span>scientist</span>
    <input type="checkbox" value="engineer" v-model="blog.categories">
    <span>engineer</span>
    <br/>
    <h2>Perview</h2>
    <div>
        <p>blog title: {{ blog.title }}</p>
        <p>blog content: </p>
        <p><pre>{{ blog.content }}</pre></p>
        <p>Checked: </p>
        <ul>
            <li v-for="category in blog.categories" :key="category.id">
                {{ category }}
            </li>
        </ul>
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            blog: {
                title: '',  
                content: '',
                categories:[]
            }
        }
    },
}
</script>

<style lang="scss" scoped>
#add-blog {
    width: 400px;
    margin:0 auto 0 auto;
    h3 {
        text-align: left;
    }
    input[type="text"] {
        width: 100%;
    }
    textarea {
        width: 100%;
        height: 60px;
    }
    > div {
        text-align: left;
        border: 1px solid grey;
    }
}
</style>
