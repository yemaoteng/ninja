<template>
  <div>
      <slot name="head-slot"></slot>
      <h1>This is son</h1>
      <slot name="foot-slot"></slot>
      <hr/>
      <h1>下面的元素使用sass来控制样式</h1>
      <div class="demo">
          <ul>
              <li></li>
          </ul>
      </div>
  </div>
</template>

<script>
</script>

<style lang="scss" scoped>
$col: #eeeeee;
h2 {
    color: $col;
}
</style>
