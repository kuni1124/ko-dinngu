<template>
  <div id="app">
    <Headers />
    <Contents />
    <Footers />
  </div>
</template>

<script>
import Headers from './components/Headers';
import Contents from './components/Contents';
import Footers from './components/Footers';

export default {
  components: { Headers, Contents, Footers }
}
</script>

<style>
  #app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
  #nav {
    padding: 30px;
  }

  #nav a {
    font-weight: bold;
    color: #2c3e50;
  }

  #nav a.router-link-exact-active {
    color: #42b983;
  }
</style>
