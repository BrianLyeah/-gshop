<template>
  <div id="app">
    <router-view/>
    <FooterGuide v-show="$route.meta.showFooter"/>
  </div>
</template>

<script>
  import FooterGuide from './components/FooterGuide/FooterGuide.vue'
  import ajax from './api/ajax.js'
  var ajax1 = ajax("aaa","",).data();


  export default {
    components:{
      FooterGuide
    }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .app
    width 400%
    height 100%
    background #f5f5f5
    color: red
    position relative
</style>
