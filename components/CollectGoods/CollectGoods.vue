<template>
<div class="collect-goods">
  <collect-goods-item :CollectGoodsInfo="CollectGoodsInfo"></collect-goods-item>
</div>
</template>

<script setup>
import {ref} from 'vue'
const CollectGoodsInfo=ref([{
  bgUrl:'https://dissrup.com/_next/image?url=https%3A%2F%2Fres.cloudinary.com%2Fdissrup%2Fimage%2Fupload%2Fv1%2Fmainnet%2Fjvmzhvlmcjeximwtrqe3%3F_a%3DATAMhAA0&w=1920&q=75',
  author:'https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmV7ncvGTm9T5ibDPANRnyCTE1iSVJuEsEJP3N1wtG3mgu&w=1920&q=75',
  name:'@vincentschwenk',
  title:'DISSRUP DEBUTS',
  artworks:'7',
  TotalSales:'0.2 ETH',
  Collected:'7'
},{
  bgUrl:'https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmSvsvZRPWUF1E8Wn5enjDBbhPur2m1hnqCbKEjCqHW16f&w=1920&q=75',
  author:'https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmXjPD9R6XmoTYiB1VtLaaPsQsa6kMZtM3izksYWbFh6kw&w=1920&q=75',
  name:'@TheInternetOffice',
  title:'ANATOMIAS AMBIVALENTES',
  artworks:'3',
  TotalSales:'',
  Collected:'1'
},{
  bgUrl:'https://image.mux.com/5OGW200mH6MLBOxU4cMsaBViwEit1jrmWTBF8AZr4ISY/thumbnail.jpg?time=0&w=1200&q=75',
  author:'https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmPZQw8noNgu7Q6pDjeJaLAhmy3uXaxiuu6ZtC2TjQyY83&w=1920&q=75',
  name:'@Forever_stu',
  title:'CHUHAISTERS 1.0',
  artworks:'10',
  TotalSales:'1.1ETH',
  Collected:'4'
},{
  bgUrl:'https://image.mux.com/5OGW200mH6MLBOxU4cMsaBViwEit1jrmWTBF8AZr4ISY/thumbnail.jpg?time=0&w=1200&q=75',
  author:'https://dissrup.com/_next/image?url=https%3A%2F%2Fipfs.infura.io%2Fipfs%2FQmZH55tes2MKqd9qEhnFxCWeVoXnqYn2QCr2vNCX3VosrQ&w=1920&q=75',
  name:'@maxsalzborn',
  title:'SALTY HEADS',
  artworks:'10',
  TotalSales:'5.3ETH',
  Collected:'8'
}])


</script>

<style lang="scss" scoped>
.collect-goods{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
</style>