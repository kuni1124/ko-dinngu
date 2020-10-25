<template>
  <div class="second-main">
      <div class="left-bars">
          <div class="gazou">
           <img src="@/assets//20200218_131059_002.jpg"/>
          </div>
          <div class="message">
           <img src="//dbcn1bdvswqbx.cloudfront.net/client_info/KITAKARO/view/userweb/images/sidebar_bnr_yakiin2016_02.jpg?timestamp=1477878765000" width="209" height="55" alt="サービス内容の詳細">
          </div>
          <div class="mitumori">
           <img src="//dbcn1bdvswqbx.cloudfront.net/client_info/KITAKARO/view/userweb/ext/t_yakiin/../../images/sidebar_bnr_yakiin2016_03.jpg?timestamp=1477878769000" width="209" height="55" alt="お見積り・お問い合わ">
          </div>
          <div class="top">
            <img src="//dbcn1bdvswqbx.cloudfront.net/client_info/KITAKARO/view/userweb/images/button_top_page.gif?timestamp=1418273553000" width="209" height="40" alt="トップページへ">
          </div>
          <div class="menu">
           <ul>
            <li ><HogeHoge name="しいたけ"></HogeHoge></li>
            <li ><HogeHoge name="しいたけ"></HogeHoge></li>
            <li><HogeHoge name="しいたけ"></HogeHoge></li>
            
           </ul>
          </div>
          
           
         
        
        <div class="insta">
          <img src="@/assets/inn.jpeg">
          <p>Instagramはこちら</p>
        </div> 
        <div class="twitter">
          <img src="@/assets/twitter.jpeg">
          <p>twitterはこちら</p>
        </div> 
       
          
      </div>
      <div class="right-bars">
        <div class="osirase">
         <div class="hogehoge"> 
         <img class="uuu" src="//dbcn1bdvswqbx.cloudfront.net/client_info/KITAKARO/view/userweb/images/top_title_topics.gif?timestamp=1418273553000">
         
         <div class="comennt-box">
          <p>[2020/10/19]※終了しました。[しいたけ]</p>
         </div>
         <div class="comennt-box">
          <p>[2020/10/19]※終了しました。[しいたけ]</p>
         </div>
         <div class="comennt-box">
          <p>[2020/10/19]※終了しました。[しいたけ]</p>
         </div>
         <div class="comennt-box">
          <p>[2020/10/19]※終了しました。[しいたけ]</p>
         </div>
         <div class="comennt-box">
          <p>自信を持っておすすめする自慢</p>
         </div>
         </div>
        </div>
        <div class="inner"> 
          <h1>人気おすすめ商品</h1>
         <div class="hako">
           <div class="setumei">
            <img src="@/assets//20200218_131059_002.jpg"/>
            <p>しいたけ</p>
            <p>地下水で組み上げた極上のしいたけを是非ご賞味してくだい。</p>
           </div>
           <div class="setumei2">
            <img src="@/assets//20200218_131059_002.jpg"/>
            <p>しいたけ</p>
            <p>地下水で組み上げた極上のしいたけを是非ご賞味してくだい。</p>
           </div>
         </div> 
        <div class="img-box">
          <div class="hoge">
           <img class="first" src="@/assets//20200829_184219.jpg">
           <img class="first" src="@/assets//20200614_174057.jpg">
         </div>
         <div class="hoge2">
           <img class="second" src="@/assets//20200829_184219.jpg">
           <img class="second" src="@/assets//20200614_174057.jpg">
           <img class="second" src="@/assets//20200614_174057.jpg">
         </div>
         <div class="hoge3">
          <img class="sard" src="@/assets//20200614_174057.jpg">
          <img class="sard" src="@/assets//20200614_174057.jpg">
         </div>
        </div>
       </div>
       </div> 
      
      
  </div>
</template>
<script>


import HogeHoge from './HogeHoge';
export default {
  components: {
   
    HogeHoge,
  },
  data() {
    return {
      isOpened: false,
      isOpened2:false,
      };
      
  },
  methods: {
    accordionToggle: function(){
      this.isOpened = !this.isOpened;
    },
    accordionToggle2: function(){
      this.isOpened2 = !this.isOpened2;
    },
    
  },
  
    


  

}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.gazou img{
  width:100%;
  height:100px;
}
.second-main {
  display: flex;
 
  margin:0 auto;
}

.left-bars{
  flex:1;
}
.right-bars{
   justify-content: space-between;
 

  
}
.hogehoge{
  width:80%;
  margin-left:10px;
  width: 580px;
}

  
.comennt-box{
 border-bottom:1px solid;
 height: 20px;
}
.right-bars p{
 
 text-align: left;
 margin-left:10px;
 
}

.hako{
  display: flex;
  

}
.setumei2{
  text-align: right;
}
  

.first{
  width:300px;
  height:150px;
  text-align:left;
}
.second{
  width:220px;
  height:115px;
  
}
.sard{
  width:335px;
  height:81px;
  
}
.img-box{
  table-layout: fixed;
  width:100%;
  height:100%;
}
.hoge{
  display: flex;
  justify-content: space-between;
}
.hoge img{
  width:280px;
}
.hoge2{
  display: flex;
  justify-content: space-between;
}
.hoge2 img{
  width:190px;
}
.hoge3{
  display: flex;
  justify-content: space-between;
}
.hoge3 img{
  display: flex;
  justify-content: space-between;
  width:280px;
}


.gazou{
  flex:1;
}
.osirase{
  width:590px;
}
.uuu{
  width:580px;
}
.setumei img{
  width: 280px;
}
.setumei2 img{
  width: 280px;
}
.js-accordion--trigger{
  width:100%;
}
.insta img{ 
  width:150px;
  height:100px;
  margin-top:30px;
  
}
.insta p{
  margin-top:0px;
}
.twitter img{
  width:150px;
  height:100px;
  margin-top:30px;
}
.twitter p{
  margin-top:0px;
}
.menu ul{
  list-style: none;
}
</style>
