<template>
  <div class="title2">
    <NuxtLayout name="common-nav">
      <template #title>
        <div class="commonnav-title">
          <p>CURATED</p>
          <p :style="{ 'margin-left': '1rem', color: 'blue' }">COLLECTIONS</p>
        </div>
      </template>
      <template #info>
        <p :style="{ 'font-size': '2.5rem' }">View all</p>
      </template>
    </NuxtLayout>
  </div>
</template>

<script setup>
import {} from "vue";
</script>

<style lang="scss" scoped>
.title2 {
  margin-top: 3rem;
  margin-bottom: 3rem;
  border-bottom:1px solid #ccc;
  .commonnav-title{
    display: flex;
    align-items: center;
    p{
      font-size: 2.5rem;
      font-weight: 600;
    }
  }
}
</style>
