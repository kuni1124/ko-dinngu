<template>
<div class=footer>
   <div class="one">
    <div class="left-bar">
     <h4>お支払い方法について</h4>
     <p>
      <a href="https://www.kitakaro.com/ext/support/index.html#creka">クレジットカード/</a><a href="https://www.kitakaro.com/ext/support/index.html#creka">コンビニ払い/</a><a href="https://www.kitakaro.com/ext/support/index.html#creka">代金引換</a>がございます。
     </p>
     <h4>送料について</h4>
     <p>お届け先１件ごとに送料を頂戴しております。<br>
        １０００円以上お買い上げで無料です。
     </p>
     <h4>お届け日について</h4>
     <img src="https://www.kitakaro.com/client_info/KITAKARO/view/userweb/images/shiteibi_info_chuigaki_330.jpg" width="330">
    </div>
    
    
    <div class="right-bar">
     <h4>お問い合わせについて</h4>
     <p>お電話からのお問い合わせ:０１２０−０００−０００</p>
     <p>メールからのお問い合わせ:user@co.jp</p>
     <h4>返品について</h4>
     <p>ご注文後のお客様都合によります返品・交換については承っておりません。万一、品質に問題がある場合は、お手数ですが北菓楼通販センター（0120-893925）までご連絡をお願いいたします。

     </p>
    </div>
   </div>
   <div class="inner">
      <h3>umekikunihiko</h3>  
    </div>
   
    <div class="container">
            <p v-on:mouseover="mouseOverAction" v-on:mouseleave="mouseLeaveAction">{{message}}</p>
            <p v-if="hoverFlag">hoverされました</p>
    </div> 
  
 </div>    
</template>
<script>

//  new Vue({
//             el: '#app',
//             data:{
//                 message: 'hoverしてください',
//                 hoverFlag: false,
//             },
//             methods: {
//                 mouseOverAction(){
//                     this.hoverFlag = true
//                 },
//                 mouseLeaveAction(){
//                     this.hoverFlag = false
//                 }
//             }
//         })
</script>
<style scoped>
.one {
    display:flex;
    justify-content: space-between;
    width:800px;
    text-align: center;
    margin:0 auto;
}
.left-bar{
    text-align:left; 
    width:400px;
    }
.left-bar h4{
    border-bottom:dotted;
}
.right-bar{
    text-align:left;
    width:400px;
}
.right-bar h4{
    border-bottom:dotted;

}
.inner{
    background: aqua;
    border: 1px solid #ccc;
}
</style>