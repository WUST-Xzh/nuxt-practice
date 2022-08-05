<template>
  <div class="goods">
    <goods-item :goodsItemInfo="goodsItemInfo"></goods-item>
  </div>
</template>

<script setup>
import { ref } from "vue";
const goodsItemInfo = ref([
  {
    description:'Caught up in Fashion',
    title:'Caught up in Fashion /  #9 Diamond',
    owner:'@chatart',
    price:'0.4 ETH',
    priceInfo:'lastPrice',
    isShow:false,
    imgUrl:
      "https://image.mux.com/ZHzKZ78XPZ78jMO9UBAzZOsJnaVNQVKgkbjKmaS6eUM/thumbnail.jpg?time=0&w=1200&q=75",
    iconUrl:
      "https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmZSvX5njHnXZLi2cCotJ4yTdpK1nFfrjC4TyRzfakD3LQ&w=1920&q=75",
    name: "@buda.tv",
  },
  {
    description:'',
    title:'EFFETE',
    owner:'@joeryba',
    price:'0.125 ETH',
    priceInfo:'reversePrice',
    isShow:true,
    imgUrl:
      "https://image.mux.com/ZHzKZ78XPZ78jMO9UBAzZOsJnaVNQVKgkbjKmaS6eUM/thumbnail.jpg?time=0&w=1200&q=75",
    iconUrl:
      "https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmZpbAG7hgid2QdpTpZfEo3FWHt2VxSKpp7qygsixbgwGi&w=1920&q=75",
    name: "@heryba",
  },
  {
    description:'',
    title:'TWO BRIDES',
    owner:'@JoshJen',
    price:'0.3 ETH',
    priceInfo:'reversePrice',
    isShow:true,
    imgUrl:
      "https://image.mux.com/ZHzKZ78XPZ78jMO9UBAzZOsJnaVNQVKgkbjKmaS6eUM/thumbnail.jpg?time=0&w=1200&q=75",
    iconUrl:
      "https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmT2MhbWABEiJD3KgSBqTvsqs8DZfvkUtjB5vjeaMETqKc&w=1920&q=75",
    name: "@JoshJen",
  },
  {
    description:'SMKLS',
    title:'ELAZAR',
    owner:'@0x8020',
    price:'0.6 ETH',
    priceInfo:'lastPrice',
    isShow:false,
    imgUrl:
      "https://image.mux.com/ZHzKZ78XPZ78jMO9UBAzZOsJnaVNQVKgkbjKmaS6eUM/thumbnail.jpg?time=0&w=1200&q=75",
    iconUrl:
      "https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmSz7AeLp2sP9GPQK5co9Pf3NuBHT8GmT8aMZoQBeFbS3G&w=1920&q=75",
    name: "@pipeled",
  },
  {
    description:'Women of Web 3.0',
    title:'CANDY FLOSS MONSTER',
    owner:'@0x8020',
    price:'0.6 ETH',
    priceInfo:'lastPrice',
    isShow:false,
    imgUrl:
      "https://image.mux.com/ZHzKZ78XPZ78jMO9UBAzZOsJnaVNQVKgkbjKmaS6eUM/thumbnail.jpg?time=0&w=1200&q=75",
    iconUrl:
      "https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmVoBAT2JPbCD6Xy65a2fhXftk9wERkwUEfG73yyCYL51b&w=1920&q=75",
    name: "@visual_citizens",
  },
  {
    description:'',
    title:'FEAR',
    owner:'@Dor_Sagiv',
    price:'0.1 ETH',
    priceInfo:'lastPrice',
    isShow:false,
    imgUrl:
      "https://image.mux.com/ZHzKZ78XPZ78jMO9UBAzZOsJnaVNQVKgkbjKmaS6eUM/thumbnail.jpg?time=0&w=1200&q=75",
    iconUrl:
      "https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmZSvX5njHnXZLi2cCotJ4yTdpK1nFfrjC4TyRzfakD3LQ&w=1920&q=75",
    name: "@nomoreluca",
  },
  {
    description:'',
    title:'ALL THAT JAZZ',
    owner:'@joangarciapons',
    price:'0.1 ETH',
    priceInfo:'lastPrice',
    isShow:false,
    imgUrl:
      "https://image.mux.com/ZHzKZ78XPZ78jMO9UBAzZOsJnaVNQVKgkbjKmaS6eUM/thumbnail.jpg?time=0&w=1200&q=75",
    iconUrl:
      "https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmYVo69B7t71R6jLCFPcm98o81P2SiFRgcPzk2hrcztioc&w=1920&q=75",
    name: "@rus1an.eth",
  },
  {
    description:'DREAMLIKE INTERIORS',
    title:'TOP OF THE MORNIN',
    owner:'@0xda8a',
    price:'0.55 ETH',
    priceInfo:'lastPrice',
    isShow:false,
    imgUrl:
      "https://image.mux.com/ZHzKZ78XPZ78jMO9UBAzZOsJnaVNQVKgkbjKmaS6eUM/thumbnail.jpg?time=0&w=1200&q=75",
    iconUrl:
      "https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmXmCbtP3TAGz7h7rokumzyXRo7yGMtbVDJwbg7MaPcnnu&w=1920&q=75",
    name: "@yamb0x",
  },
  {
    description:'',
    title:'PURE SOUL',
    owner:'@kanneryilmaz',
    price:'',
    priceInfo:'lastPrice',
    isShow:false,
    imgUrl:
      "https://image.mux.com/ZHzKZ78XPZ78jMO9UBAzZOsJnaVNQVKgkbjKmaS6eUM/thumbnail.jpg?time=0&w=1200&q=75",
    iconUrl:
      "https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmTt3h4gwSk9HpBEMxR588JzSKSj6X529A7suwcicwqCfF&w=1920&q=75",
    name: "@mrjuliang",
  },
]);
</script>

<style lang="scss" scoped>
.goods {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  margin-top: 8rem;
}
</style>
