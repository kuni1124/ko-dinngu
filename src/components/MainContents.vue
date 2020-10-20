<template>
  <div class="main">
    <div class="image">
     <ul>
      <li><img src="@/assets//20191129_200605_001.jpg"/></li>
      
     </ul>
    </div>
      <div class="navi">
        <ul>
         <li>特集</li>
         <li>生椎茸</li>
         <li>極小椎茸</li>
         <li>干し椎茸</li>
        </ul>
      </div>
    </div>
    
  
</template>

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
.image img{
  width:100%;
  height:500px;
  
}
.image ul{
  list-style:none;
  margin:0px;
  padding:0px;
}


</style>
