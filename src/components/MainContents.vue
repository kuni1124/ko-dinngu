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
        <div class="container">
            
           
    </div> 
        <ul>
          
         <li><Hoge name="特集"></Hoge></li>
         <li><Hoge name="しいたけ"></Hoge></li>
         <li>干し椎茸</li>
        </ul>
      </div>
    </div>
    
  
</template>
<script>
import {
  Hooper,
  Slide,
 
  } from 'hooper';
import 'hooper/dist/hooper.css';
import Hoge from './Hoge';

export default {
  components: {
    Hooper,
    Slide,
    Hoge
  },
  
  data() {
    return {
      hoverFlag: false,
      hoverFlag2: false,
      message: 'hoverしてください',
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
  }, 
  }

</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.navi ul {
  list-style:none;
  display:flex;
  background-color: blue;
  color: antiquewhite;
  
}
.navi li{
  width: 100%;
  table-layout: fixed;
}

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
}

</style>
