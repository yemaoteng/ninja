<template>
  <div>
      <slot name="head-slot"></slot>
      <h1>This is son</h1>
      <slot name="foot-slot"></slot>
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
