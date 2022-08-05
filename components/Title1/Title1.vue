<template>
  <div class="title1">
    <NuxtLayout name="common-nav">
      <template #title>
        <div class="shine-circle"></div>
        <div class="commonnav-title">
          <p>TRENDING</p>
          <p :style="{'margin-left':'1rem','color':'blue'}">ACTIVITY</p>
        </div>
      </template>
      <template #info>
        <p :style="{'font-size':'2.5rem'}">View all</p>
      </template>
    </NuxtLayout>
  </div>
</template>

<script>
export default {
  layout: false,
};
</script>

<style lang="scss" scoped>
.title1 {
  margin-top: 7rem;
  .shine-circle {
    width: 1.3rem;
    aspect-ratio: 1;
    border-radius: 50%;
    background-color: blue;
    animation: shine 1.8s infinite linear;
  }
  .commonnav-title{
    margin-left: 1rem;
    display: flex;
    align-items: center;
    p{
      font-size: 2.5rem;
      font-weight: 600;
    }
  }
}

@keyframes shine {
  0% {
    opacity: 1;
  }
  25% {
    opacity: 0.5;
    transform: scale(0.8);
  }
  50% {
    opacity: 0;
    transform: scale(0.6);
  }
  75% {
    opacity: 0.5;
    transform: scale(0.8);
  }
  100% {
    opacity: 1;
  }
}
</style>
