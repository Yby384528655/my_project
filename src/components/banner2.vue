<template>
  <div class="page-swipe">
    <mt-swipe :auto="4000">
    	<mt-swipe-item v-for="item in items" v-bind:class=item.className>
    		<slot></slot>
    	</mt-swipe-item>
	</mt-swipe>
  </div>
</template>

<script>
export default {
  name: 'page-swipe',
  data () {
    return {
    	items:[
    		{id:1,className:'slide1',content:'hello',img:'./src/assets/banner1.png'},
    		{id:2,className:'slide2',content:'hi',img:'assets/banner2.png'},
    		{id:3,className:'slide3',content:'go',img:'src/assets/banner3.png'}]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
.page-swipe .mint-swipe {
    height: 200px;
    color: #fff;
    font-size: 30px;
    text-align: center;
    margin-bottom: 20px;
}
.page-swipe .mint-swipe-item {
    line-height: 200px;
}
.page-swipe .slide1 {
    background-color: #0089dc;
    color: #fff;
}
.page-swipe .slide2 {
    background-color: #ffd705;
    color: #000;
}
.page-swipe .slide3 {
    background-color: #ff2d4b;
    color: #fff;
}
.page-swipe-desc {
    text-align: center;
    color: #666;
    margin-bottom: 5px;
}
</style>
