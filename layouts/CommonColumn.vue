<template>
<div class="common-column">
  <div class="left">
    <slot name="left"></slot>
  </div>
  <div class="middle">
     <slot name="middle"></slot>
  </div>
  <div class="right">
      <slot name="right"></slot>
  </div>
</div>
</template>

<script setup>
import {} from 'vue'
</script>

<style lang="scss" scoped>
.common-column{
  width: 50rem;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
</style>