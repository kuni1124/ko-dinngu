<template>
     <div class="js-accordion" v-cloak>
         <button class="js-accordion--trigger" type="button" :class="{ '_state-open': isOpened }" @click="accordionToggle()">{{name}}
           
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
        <button class="js-accordion--trigger" type="button" :class="{ '_state-open': isOpened2 }" @click="accordionToggl()">{{name}}
           
           <!-- v-showは=の中身がtureだったら表示 !は反転-->
          <span v-if="isOpened2">-</span> 
          <span v-else>+</span>
         </button>
           <!-- isOpened -->
        <div class="js-accordion--target" :class="{ '_state-open': isOpened2 }" v-if="isOpened2">
         <div class="js-accordion--body">
           <ul>
             <li>bbb</li>
             <li>aaa</li>
             <li>aaa</li>
             <li>aaa</li>
             <li>aaa</li>
             <li>aaa</li>
           </ul>    
         </div>
        </div>
       </div>
       
       
</template>
<script>

export default {
  components: {
    
   
  },
  props: ['name'],
  data() {
    return {
      isOpened: false,
      isOpened2: false,
      };
      
  },
  methods: {
       accordionToggle: function(){
      this.isOpened = !this.isOpened;
    },
       accordionToggl: function(){
      this.isOpened2 = !this.isOpened2;
    },
     
    }, 
  }

</script>