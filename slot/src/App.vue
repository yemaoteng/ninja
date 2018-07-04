<template>
  <div>
    <app-son>
      <h2 slot="head-slot">今日头条要打架！</h2>
      <p slot="table-slot">报表</p>
      <p slot="foot-slot">记者：路小花</p>
    </app-son>
    <app-son>
      <h2 slot="head-slot">腾讯股价大涨</h2>
      <p slot="table-slot">利好信息列表</p>
      <p slot="foot-slot" class="editor">记者：王小明</p>
    </app-son>
  </div>
</template>

<script>
import son from "./components/son.vue";

export default {
  components: {
    "app-son": son
  }
};
</script>

<style scoped>
.editor {
  color: red;
}
</style>
