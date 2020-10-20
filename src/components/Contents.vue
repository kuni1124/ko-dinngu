<template>
  <div class="container">
    <SideBars />
    <MainContents />
    <SideBarsa />
    
    <button @click="click">aaa</button>
  </div>
</template>

<script>
import MainContents from './MainContents';
import SideBars from './SideBars';
import SideBarsa from './SideBarsa';


export default {
  components: { MainContents, SideBars, SideBarsa, },
  methods: {
    click() {
      alert('hellow');
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
