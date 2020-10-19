<template>
  <div class="container">
    <SideBars />
    <MainContents />
    <button @click="click">aaa</button>
  </div>
</template>

<script>
import MainContents from './MainContents';
import SideBars from './SideBars';

export default {
  components: { MainContents, SideBars },
  methods: {
    click() {
      alert('hellow');
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  display: flex;
}
</style>
