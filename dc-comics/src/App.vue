<script>

import SiteHeader from './components/SiteHeader.vue';
import SiteMain from './components/SiteMain.vue';
import SiteFooter from './components/SiteFooter.vue';

export default{
  name: 'App',
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter
  }
}


</script>

<template>

  <!-- header -->
  <SiteHeader/>

  <!-- main -->
  <SiteMain/>

  <!-- footer -->
  <SiteFooter/>
  
</template>

<style scoped>
</style>
