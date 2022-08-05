<template>
  <div class="NavBar">
    <div class="NavBar-logo">
      <img src="../../assets/img/logo.png" />
    </div>
    <form action="" class="NavBar-form">
      <div class="NavBar-search">
        <div class="search-icon">
          <svg
            t="1659064079426"
            class="icon"
            viewBox="0 0 1024 1024"
            version="1.1"
            xmlns="http://www.w3.org/2000/svg"
            p-id="3134"
            width="20"
            height="20"
          >
            <path
              d="M789.804097 737.772047 742.865042 784.699846 898.765741 940.600545 945.704796 893.672746Z"
              p-id="3135"
            ></path>
            <path
              d="M456.92259 82.893942c-209.311143 0-379.582131 170.282245-379.582131 379.582131s170.270988 379.570875 379.582131 379.570875c209.287607 0 379.558595-170.270988 379.558595-379.570875S666.210197 82.893942 456.92259 82.893942zM770.128989 462.477097c0 172.721807-140.508127 313.229934-313.206398 313.229934-172.720783 0-313.229934-140.508127-313.229934-313.229934s140.508127-313.229934 313.229934-313.229934C629.620861 149.247162 770.128989 289.75529 770.128989 462.477097z"
              p-id="3136"
            ></path>
          </svg>
        </div>
        <input
          type="text"
          placeholder="Search for artworks, collections, artists etc"
        />
      </div>
    </form>

    <div class="NavBar-title">
      <span v-for="item in titles">{{ item }}</span>
    </div>

    <div class="NavBar-connect">Connect</div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const titles = ref(["Explore", "Drops", "Community"]);
</script>

<style lang="scss" scoped>
.NavBar {
  box-sizing: border-box;
  height: 10rem;
  padding: 2rem 8rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  .NavBar-form {
    padding: 0.7rem 1rem;
    background-color: #edf2f7;
    border-radius: 1rem;
    .NavBar-search {
      width: 46rem;
      display: flex;
      align-items: center;
      .search-icon {
        width: 5.1rem;
        height: 4.6rem;
        position: relative;
        svg {
          position: absolute;
          left: 50%;
          top: 50%;
          transform: translate(-50%, -50%);
        }
      }
      input {
        width: 90%;
        height: 4.6rem;
        border: 0;
        background-color: #edf2f7;
        font-size: 1.6rem;
        outline: none;
      }
    }
  }
  .NavBar-title {
    width: 36rem;
    height: 2.3rem;
    display: flex;
    justify-content: space-between;
    span {
      font-size: 2rem;
      color: #999fa6;
    }
  }
  .NavBar-connect{
    font-size: 2rem;
    border: 1px solid #000;
    padding: 0.9rem 2.8rem;
    border-radius: 2.8rem;
  }
}
</style>
