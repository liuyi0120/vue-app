<template>
  <div id="app">
    <router-view/>
    <FooterNav/>
  </div>

</template>

<script type="text/ecmascript-6">
import FooterNav from './components/FooterNav/FooterNav'
  export default {
    components:{
      FooterNav
    }
  }
</script>

<style lang="stylus" rel="stylesheet/stylus" scoped>
 
</style>
