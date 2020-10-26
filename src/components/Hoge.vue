<template>
     <div class="drop" v-on:mouseover="mouseOverAction" v-on:mouseleave="mouseLeaveAction">{{name}}
      <div class="dropdown" v-if="hoverFlag">hoverされました</div>
     </div>
     
</template>
<script>

export default {
  components: {
    
   
  },
  props: ['name'],
  data() {
    return {
      hoverFlag: true,
      
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
     
    }, 
  }

</script>
<style scoped>
.drop{
  position: relative;
}
.dropdown {
    position: absolute;
    top: 100%;
    left: 0;
    display: none;
    padding: 0;
    list-style-type: none;
    background-color: #007db9;
    height: 50px;
}
</style>