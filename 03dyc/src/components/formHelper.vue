<template>
    <div>
        <slot name="form-header"></slot>
        <slot name="form-p"></slot>
        <p for="name">Name:</p>
        <input type="text" name="name" placeholder="Please enter your name" />
        <br/>
        <p for="phone">Phone:</p>
        <input type="text" name="phone" placeholder="Please enter your phone"/>
        <slot name="form-footer"></slot>
    </div>
</template>

<script>
export default{

}
</script>

<style lang="scss" scoped>
div {
    padding: 20px;
    margin-top: 50px;
    p {
        width:100%;
        text-align: left;
        padding:0;
        margin:10px 0 0 0;
        line-height: 20px;
        &:first-of-type {
            color:crimson;
            text-align: center;
        }
    }
    input {
        width: 100%;
    }
    p:last-of-type{
        color:grey;
        text-align: right;
        font-size: 11px;
    }
}
</style>
