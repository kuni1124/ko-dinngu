<template>
  <div class="main">
    <div class="image">
     
 <hooper :progress="true" :autoPlay="true" :playSpeed="2000">
  <slide>
    <img src="@/assets//20191129_200605_001.jpg" >
  </slide>
  <slide>
   <img src="@/assets//20200614_174057.jpg"/>
  </slide>
  <slide>
    <img src="@/assets//20200829_184219.jpg"/>
  </slide>
  
</hooper>
     
    </div>
      <div class="navi">
            <div class="drop" v-on:mouseover="mouseOverAction" v-on:mouseleave="mouseLeaveAction">特集
            <div class="dropdown" v-if="hoverFlag">
               <ul>
                 <li v-for="item in items" :key = 'item'>
                   <a v-bind:href="item.url" target="_blank">{{ item.text }}</a>
                </li>
               </ul> 
            </div>
            </div>
            <div class="drop" v-on:mouseover="mouseOverAction2" v-on:mouseleave="mouseLeaveAction2">しいたけ
            <div class="dropdown" v-if="hoverFlag2">
              <ul>
                 <li v-for="item in items" :key = 'item'>
                   <a v-bind:href="item.url" target="_blank">{{ item.text }}</a>
                </li>
               </ul> 
            </div>
            </div>
            <div class="drop" v-on:mouseover="mouseOverAction3" v-on:mouseleave="mouseLeaveAction3">干ししいたけ
            <div class="dropdown" v-if="hoverFlag3">
              <ul>
                 <li v-for="item in items" :key = 'item'>
                   <a v-bind:href="item.url" target="_blank">{{ item.text }}</a>
                </li>
               </ul> 
            </div>
            </div>
            <div class="drop" v-on:mouseover="mouseOverAction4" v-on:mouseleave="mouseLeaveAction4">訳あり
            <div class="dropdown" v-if="hoverFlag4">
              <ul>
                 <li v-for="item in items" :key = 'item'>
                   <a v-bind:href="item.url" target="_blank">{{ item.text }}</a>
                </li>
               </ul> 
            </div>
            </div>
               
    </div>
   </div>
    
  
</template>
<script>
import {
  Hooper,
  Slide,
 
  } from 'hooper';
import 'hooper/dist/hooper.css';
//import Hoge from './Hoge';

export default {
  components: {
    Hooper,
    Slide,
    //Hoge
  },
  
  data() {
    return {
      hoverFlag: false,
      hoverFlag2: false,
      hoverFlag3: false,
      hoverFlag4: false,
      items:[
          {
            url: 'http://www.google.com/',
            text: 'google'
          },
          {
            url: 'http://www.yahoo.co.jp/',
            text: 'yahoo'
          }
        ],
      };
      
      
  },
  methods: {
      mouseOverAction(){
          this.hoverFlag = true
                },
      mouseLeaveAction(){
          this.hoverFlag = false
    },
      mouseOverAction2(){
          this.hoverFlag2 = true
                },
      mouseLeaveAction2(){
          this.hoverFlag2 = false
    },
      mouseOverAction3(){
          this.hoverFlag3 = true
                },
      mouseLeaveAction3(){
          this.hoverFlag3 = false
    },
      mouseOverAction4(){
          this.hoverFlag4 = true
                },
      mouseLeaveAction4(){
          this.hoverFlag4 = false
    },
  }, 
  }

</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>



.hooper img{
  width:800px;
  height:100%;
}
.image ul{
  list-style:none;
  margin:0px;
  padding:0px;
}
.main{
  text-align: center;
}.navi{
  display: flex;
  
  background: aqua;
  }
  .drop{
  position: relative;
  margin-left:120px;
}
.dropdown {
    position: absolute;
    top: 100%;
    left: 0;   
    padding: 0;
    list-style-type: none;
    background-color: #007db9;
    height: 100px;
    width: 150px;
   border-bottom: 1px solid #fff;
}
</style>
