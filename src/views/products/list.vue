<template>
   
<div data-v-320224c2="" data-v-40b8d964="" class="row" data-v-35ea163e="" style="padding-left:1px;padding-right:1px;" id="div2">

    <item v-for="(post, index) in posts" :key="index" :post="post" />
    
  </div>
  
</template>

<script>
import item from "./item.vue"
export default {
  props: {
    posts: {
      type: Array,
      required: true,
    },
  },
  methods:{
    add2cart(){
      console.log("list");
      this.$parent.add2cart();
    },
  },
  components: {
    item,
  },
}
</script>

<style>
#div2{
width: 100%; max-width: 1100px; padding: 22px;margin-top: 20px; margin-right: auto; margin-left: auto;  box-shadow: 0px 8px 22px #00000036;
}
</style>