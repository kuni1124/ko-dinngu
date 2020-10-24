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
        <div class="js-accordion" v-cloak>
         <button class="js-accordion--trigger" type="button" :class="{ '_state-open': isOpened }" @click="accordionToggle()">
           しいたけ
           <!-- v-showは=の中身がtureだったら表示 !は反転-->
          <span v-if="isOpened">-</span> 
          <span v-else>+</span>
         </button>
           <!-- isOpened -->
        <div class="js-accordion--target" :class="{ '_state-open': isOpened }" v-if="isOpened">
         <div class="js-accordion--body">
           <ul>
             <li>aaa</li>
             <li>aaa</li>
             <li>aaa</li>
             <li>aaa</li>
             <li>aaa</li>
             <li>aaa</li>
           </ul>    
         </div>
        </div>
       </div>
       <div class="js-accordion2" v-cloak>
         <button class="js-accordion--trigger2" type="button" :class="{ '_state-open': isOpened2 }" @click="accordionToggle2()">
           しいたけ
           <!-- v-showは=の中身がtureだったら表示 !は反転-->
          <span v-if="isOpened2">-</span> 
          <span v-else>+</span>
         </button>
           <!-- isOpened -->
        <div class="js-accordion--target2" :class="{ '_state-open': isOpened2 }" v-if="isOpened2">
         <div class="js-accordion--body2">
           <ul>
             <li>aaa</li>
             <li>aaa</li>
             <li>aaa</li>
             <li>aaa</li>
             <li>aaa</li>
             <li>aaa</li>
           </ul>    
         </div>
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
       
          
      </div>
      <div class="right-bars">
        <div class="osirase">
         <img src="//dbcn1bdvswqbx.cloudfront.net/client_info/KITAKARO/view/userweb/images/top_title_topics.gif?timestamp=1418273553000" width="677" height="42" alt="トピックス｜TOPICS">
      
         <h3>[2020/10/19]※終了しました。[しいたけ]</h3>
         <h3>[2020/10/19]※終了しました。[しいたけ]</h3>
         <h3>[2020/10/19]※終了しました。[しいたけ]</h3>
         <h3>[2020/10/19]※終了しました。[しいたけ]</h3>
        </div>
        <div class="inner"> 
          <p>自信を持っておすすめする自慢</p>
          <h1>人気おすすめ商品</h1>
         <div class="box"> 
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
        
      </div >
      
  </div>
</template>
<script>

 

export default {
  
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
  width: 800px;
  margin:0 auto;
}
.right-bars h3{
 border-bottom:1px solid;
}
.box{
  display: flex;
}
  
.box img{
  width:300px;
  height:200px;
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
.osirase img{
  width:590px;
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
</style>
