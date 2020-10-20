<template>
<div class="box">
    <h1>umekikuni</h1>
     <div class="support-list">
       <div class="gaido">
        <ul>
         <li>ご利用ガイド</li>
         <li>お問い合わせ</li>
         <li>ヘルプ</li>
         <li>ガイド</li>
        </ul>
       </div>
     
       <div class="login-bar">
        <ul>
         <div class="search">
          <li>
           <input name="keyworc" id="form" value type="text" class="sidebar-form" placeholder="商品名で検索が可能です">
          </li>
          <li>
           <input src="//dbcn1bdvswqbx.cloudfront.net/client_info/KITAKARO/view/userweb/images/sidebar_button_search.jpg?timestamp=1507718595000" type="image" class="button" alt="商品名で検索が可能です">
          </li>

          <li>
           <img src="//dbcn1bdvswqbx.cloudfront.net/client_info/KITAKARO/view/userweb/images/header_button_login.gif?timestamp=1418273553000" alt="ログイン" width="99" height="26">
          </li>
          <li>
           <img src="//dbcn1bdvswqbx.cloudfront.net/client_info/KITAKARO/view/userweb/images/header_button_member.gif?timestamp=1418273553000" alt="新規会員登録" width="135" height="26">
          </li>
         </div>
       </ul>
     </div>
    </div>
     
</div>  
  
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.box {
  display: flex;
  width: 320px;
}
.support-list ul{ 
  display: flex;
  list-style: none;
  width: 800px;
}
.search{ 
  display: flex;
  list-style: none;
  width: 800px;
}
.search img{
  margin-left:10px;
}
.gaido li{
  width: 100%;
  table-layout: fixed;
}
.login-bar{
  margin-left:100px;
}

</style>
