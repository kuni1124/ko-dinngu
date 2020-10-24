<template>
  <div class="container">
    <SideBars />
    <MainContents />
    <SideBarsa />
    
   
    
   
  </div>
</template>
<script>
import MainContents from './MainContents';
import SideBars from './SideBars';
import SideBarsa from './SideBarsa';


export default {
  components: { MainContents, SideBars, SideBarsa, },
 
  }

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container{
  width:800px;
  text-align: center;
  margin:0 auto;

}
</style>
