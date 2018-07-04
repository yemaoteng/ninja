<template>
  <div>
    <slot name="head-slot"></slot>    
    <slot name="table-slot"></slot>
    <div class="demo">
        <ul>
            <li>li</li>
            <li>li</li>
            <li>li</li>
        </ul>
    </div>
    <slot name="foot-slot" class="editor"></slot>
    <hr/> 
  </div>
</template>

<script>
</script>

<style lang="scss" scoped>
$col: blue;
@mixin no-bullets {
    list-style: none;
    li {
        list-style-image: none;
        list-style-type: none;
        margin-left: 0px;
}}
h2 {
    color: $col;
    text-align: center;
}
.demo {
    ul {
        @include no-bullets();
        position: relative;
        border: 1px solid green;
        li {
            line-height: 30px;
            position: relative;
            color:green;
            &::after {
                content:'';
                position: absolute;
                left: -15px;
                top: 10px;
                width: 10px;
                height: 10px;
                background-color: grey;
                z-index: 1;
                border-radius: 50%;
            }
        }
    }
}
.editor {
    text-align: right;
}
</style>
