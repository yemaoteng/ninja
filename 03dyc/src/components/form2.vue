<template>
<formHelper>
    <h1 slot="form-header">阿里职位招聘</h1>
    <p slot="form-p">秋招即将开始</p>
    <p slot="form-footer">记者：王二明</p>
</formHelper>
</template>

<script>
import formHelper from './formHelper';

export default {
    components: {
        formHelper: formHelper
    }
}
</script>
