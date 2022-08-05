<template>
  <div class="HomeBanner">
    <div class="HomeBanner-left">
      <div class="HomeBanner-left-top">
        <img
          src="https://dissrup.com/_next/image?url=https%3A%2F%2Fres.cloudinary.com%2Fdissrup%2Fimage%2Fupload%2Fv1%2Fmainnet%2Fjvmzhvlmcjeximwtrqe3%3F_a%3DATAMhAA0&w=1920&q=75"
        />
        <p>Dissrup Debuts</p>
      </div>
      <div class="HomeBanner-left-middle">
        <p class="HomeBanner-left-middle-title">Sometimes Colorful</p>
        <div class="HomeBanner-left-middle-author">
          <p
            :style="{
              'font-size': '1.8rem',
              'font-weight': '500',
              'margin-right': '0.5rem',
            }"
          >
            by
          </p>
          <p :style="{ 'font-size': '1.8rem', color: '#ccc' }">
            Santi Zoraidez
          </p>
        </div>
        <!-- 横线 -->
        <div
          :style="{
            width: '44rem',
            'border-bottom': '1px solid #000',
            'margin-top': '2rem',
          }"
        ></div>
        <div class="HomeBanner-left-middle-info">
          <div class="HomeBanner-left-middle-info-left">
            <p :style="{ 'font-size': '1.2rem', 'line-height': '1.6rem' }">
              Reserve Price:
            </p>
            <p :style="{ 'font-size': '2.5rem', 'font-weight': '500' }">
              1.0 ETH
            </p>
            <p :style="{ color: '#ccc' }">$1727.61</p>
            <!-- 竖线 -->
          </div>
          <div
            :style="{
              height: '5rem',
              'border-right': '0.1rem solid #ccc',
              'margin-right': '1rem',
            }"
          ></div>
          <div class="HomeBanner-left-middle-info-right">
            <p :style="{ 'margin-bottom': '1.8rem' }">Owned by:</p>
            <div class="author">
              <div class="circle"></div>
              <p :style="{ 'marign-left': '0.5rem' }">@szodaidez</p>
            </div>
          </div>
        </div>
      </div>
      <div class="HomeBanner-left-bottom">Place a bid</div>
    </div>
    <div class="HomeBanner-right">
      <img src="https://image.mux.com/ls026Kua7UYZuJYdN2YAjxiSRuyGG8HoEgLKs5mDWF7E/thumbnail.jpg?time=0&w=1200&q=75"/>
    </div>
  </div>
</template>

<script setup>
import {} from "vue";
</script>

<style lang="scss" scoped>
.HomeBanner {
  margin-top: 2.5rem;
  height: 70rem;
  display: flex;
  justify-content: center;
  align-items: center;
  .HomeBanner-left {
    box-sizing: border-box;
    width: 64rem;
    padding: 0.4rem 6.4rem 0 6.4rem;
    .HomeBanner-left-top {
      display: flex;
      align-items: center;
      justify-content: flex-start;
      padding: 1rem 0;
      img {
        width: 2.5rem;
        aspect-ratio: 1;
        border-radius: 50%;
        margin-right: 0.8rem;
      }
    }
    .HomeBanner-left-middle {
      .HomeBanner-left-middle-title {
        font-family: "Apoc Revelations", Georgia, serif;
        font-weight: 500;
        word-break: keep-all;
        font-size: 7.2rem;
        line-height: 6rem;
        letter-spacing: -0.02rem;
      }
      .HomeBanner-left-middle-author {
        display: flex;
        justify-content: flex-start;
        align-items: center;
        margin-top: 1rem;
      }
      .HomeBanner-left-middle-info {
        display: flex;
        align-items: center;
        margin-top: 2rem;
        .HomeBanner-left-middle-info-left {
          padding-right: 4.6rem;
        }
        .HomeBanner-left-middle-info-right {
          padding-left: 3.6rem;
          .author {
            display: flex;
            align-items: center;
            background-color: #f8f8f8;
            padding: 0.3rem 0.6rem;
            border-radius: 2.5rem;
            .circle {
              width: 2.6rem;
              aspect-ratio: 1;
              border-radius: 50%;
              background-color: #ccc;
              margin-right: 0.5rem;
            }
          }
        }
      }
    }
    .HomeBanner-left-bottom {
      margin-top: 6rem;
      width: 44rem;
      height: 5rem;
      line-height: 5rem;
      background-color: #000;
      font-size: 2rem;
      font-weight: 600;
      color: #fff;
      text-align: center;
      border-radius: 5rem;
    }
  }
  .HomeBanner-right {
    width: 64rem;
    height: 70rem;
    img{
      width: 90%;
      height: 100%;
    }
  }
}
</style>
