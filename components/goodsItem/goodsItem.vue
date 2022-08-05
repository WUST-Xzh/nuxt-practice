<template>
  <div class="goodsItem" v-for="item in goodsItemInfo">
  <div class="content">
    <!-- 顶部 -->
    <div class="top">
      <div class="top-left">
        <img :src="item.iconUrl" />
        <span :style="{ 'margin-left': '0.5rem' }" class="authorName">{{
          item.name
        }}</span>
      </div>
      <div class="top-right">
        <div class="click" :style="{ color: 'blue', 'font-weight': '600' }">
          + Follow
        </div>
      </div>
    </div>
    <!-- 中间内容 -->
    <img class="middle" :src="item.imgUrl" />
    <!-- 底部信息 -->
    <div class="bottom">
      <div class="bottom-top">
        <p :style="{ color: '#ccc' }">{{ item.description }}</p>
        <p class="title">{{ item.title }}</p>
      </div>
      <div class="bottom-bottom">
        <div class="bottom-bottom-left">
          <p :style="{ color: '#ccc', 'line-height': '1.8rem' }">Owner</p>
          <div class="owner">
            <p></p>
            <p>{{ item.owner }}</p>
          </div>
        </div>
        <div class="bottom-bottom-right">
          <div class="lastPrice" v-if="item.priceInfo=='lastPrice'">
            <span :style="{'color':'#ccc'}">Last sold for </span>
            <span>{{item.price}}</span>
          </div>
          <div v-else class="reservePrice">
            <p :style="{ color: '#ccc', 'line-height': '1.8rem' }">Reserve price</p>
            <p :style="{'line-height': '2rem'}">{{item.price}}</p>
          </div>
          <button v-if="item.isShow">Place Bid</button>
          
        </div>
      </div>
    </div>
  </div>
  </div>
    
</template>

<script>
export default {
  props: ["goodsItemInfo"]

};
</script>

<style lang="scss" scoped>
.goodsItem {
  width: 44rem;
  height: 66.2rem;
  padding: 0 2rem;
  box-sizing: border-box;
  .content{
    width: 40rem;
    height: 60.2rem;
    border: 1px solid #ccc;
    border-radius: 1rem;
  }
  .top {
    box-sizing: border-box;
    padding: 0 1rem;
    width: 100%;
    height: 5.9rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
    align-items: center;
    .top-left {
      display: flex;
      align-items: center;
      img {
        width: 2.7rem;
        aspect-ratio: 1;
        border-radius: 50%;
      }
    }
  }
  .middle {
    width: 40rem;
    height: 40rem;
  }
  .bottom {

    .bottom-top {
      height: 5rem;
      padding: 0 1.5rem;
      position: relative;
      p {
        &:first-child {
          margin-top: 1rem;
          width: 100%;
          line-height: 1.8rem;
        }
        &:nth-child(2) {
          position: absolute;
          top: 2rem;

          font-size: 2rem;
          font-weight: 700;
          white-space: nowrap;
          overflow: hidden;
          text-overflow: ellipsis;
        }
      }
    }
    .bottom-bottom {
      margin-top: 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 0 1.5rem;
      .bottom-bottom-left {
        .owner {
          display: flex;
          align-items: center;
          p {
            &:first-child {
              width: 2rem;
              aspect-ratio: 1;
              border-radius: 50%;
              background-color: #ccc;
              margin-right: 0.5rem;
            }
            &:nth-child(2) {
              line-height: 3rem;
            }
          }
        }
      }
      .bottom-bottom-right{
        height: 3.2rem;
        display: flex;
        align-items: flex-end;
        .reservePrice{
          width: 8rem;
          margin-right: 0.2rem;
        }
        button{
          background-color: #fff;
          height: 3.3rem;
          padding: 0 2rem;
          border-radius: 4rem;
        }
      }
    }
  }
}
</style>
