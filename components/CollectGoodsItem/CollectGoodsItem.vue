<template>
  <div
    class="collect-goods-item"
    v-for="item in CollectGoodsInfo"
    :style="{
      background: 'url(' + item.bgUrl + ') no-repeat',
      'background-size': '58.2rem 62.2rem',
    }"
  >
    <!-- 分为上下布局 -->
    <div class="collect-goods-item-top">
      <div class="author">
        <img :src="item.author" />
        <span
          :style="{
            'margin-left': '0.5rem',
            color: '#fff',
            'font-weight': '600',
          }"
          >{{ item.name }}</span
        >
      </div>
      <p class="title">{{ item.title }}</p>
    </div>
    <div class="collect-goods-item-bottom">
      <NuxtLayout name="common-column">
        <template #left>
          <p class="head">Artworks</p>
          <p class="number">{{item.artworks}}</p>
        </template>
        <template #middle>
          <p v-if="item.TotalSales" class="head">TotalSales</p>
          <p class="number">{{ item.TotalSales }}</p>
        </template>
        <template #right>
          <p class="head">Collected by ({{ item.Collected }})</p>
        </template>
      </NuxtLayout>
    </div>
  </div>
</template>

<script>
export default {
  props: ["CollectGoodsInfo"],
  layout: false,
};
</script>

<style lang="scss" scoped>
.collect-goods-item {
  width: 58.2rem;
  aspect-ratio: 1;
  position: relative;
  border-radius: 2rem;
  margin: 2rem 2rem;
  .collect-goods-item-top {
    position: absolute;
    left: 3rem;
    bottom: 20rem;
    .author {
      width: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 0.5rem 0.6rem;
      border-radius: 2rem;
      background: rgba(#d9d9d9, 0.8);
      img {
        width: 2.6rem;
        aspect-ratio: 1;
        border-radius: 50%;
        z-index: 999;
      }
    }
    .title {
      font-size: 3rem;
      padding: 3rem 0;
      width: 30rem;
      color:#fff;
      font-weight: 700;
    }
  }
  .collect-goods-item-bottom{
    position: absolute;
    left: 3rem;
    bottom: 6rem;
    padding: 3rem 1rem;
    border-radius: 2rem;
    background: rgba(#d9d9d9, 0.7);
    .head{
      font-size: 1.5rem;
      color: #fff;
      font-weight: 500;
    }
    .number{
      font-size: 2.5rem;
      color: #fff;
      font-weight: 500;
      margin-top: 0.5rem;
    }
  }
}
</style>
