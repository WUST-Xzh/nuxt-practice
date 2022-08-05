<template>
<div class="CommonNavBar">
  <div class="NavBar-left">
    <slot name="title"></slot>
  </div>
  <div class="NavBar-right">
    <slot name="info"></slot>
  </div>
</div>
</template>

<style lang="scss" scoped>
.CommonNavBar{
  height: 3.75rem;
  display:flex;
  justify-content: space-between;
  align-items: center;
  padding: 0 10rem;
  .NavBar-left{
    display: flex;
    align-items: center;
  }
}
</style>