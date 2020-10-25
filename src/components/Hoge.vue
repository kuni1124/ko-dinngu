<template>
     <div v-on:mouseover="mouseOverAction" v-on:mouseleave="mouseLeaveAction">{{name}}
     <p v-if="hoverFlag">hoverされました</p>
     </div>
     
</template>
<script>

export default {
  components: {
    
   
  },
  props: ['name'],
  data() {
    return {
      hoverFlag: false,
      
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