<template>
<div id="add-blog">
    <h1>Add Blog Page</h1>
    <h3>Blog title</h3>
    <input type="text" v-model="blog.title"/>
    <h3>Blog content</h3>
    <textarea v-model="blog.content"/>
    <h3>Jobs: </h3>
    <input type="checkbox" value="ninja" v-model="blog.categories">
    <span>ninja</span>
    <input type="checkbox" value="wizard" v-model="blog.categories">
    <span>wizard</span>
    <input type="checkbox" value="scientist" v-model="blog.categories">
    <span>scientist</span>
    <input type="checkbox" value="engineer" v-model="blog.categories">
    <span>engineer</span>
    <h3>Author: </h3>
    <select v-model="blog.author">
        <option v-for="author in authors" :key="author.id">
            {{ author }}
        </option>
    </select>
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
        <p>Author: {{ blog.author }}</p>

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
                categories:[],
                author:'',
            },
            authors:['zhao','qian','sun','li']

        }
    },
}
</script>

<style lang="scss" scoped>
#add-blog {
    width: 400px;
    margin:0 auto 0 auto;
    text-align: left;
    h1,h2 {
        text-align: center;
    }
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
