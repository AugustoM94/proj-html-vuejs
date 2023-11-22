<template>
    <HeaderAppUp/>
    <HeaderAppDown />
    <OurHistoryApp/>
</template>

<script>

import HeaderAppUp from './components/HeaderAppUp.vue';
import HeaderAppDown from './components/HeaderAppdown.vue';
import OurHistoryApp from './components/OurHistoryApp.vue';


  export default {
    name: 'App',
  components: {
    HeaderAppUp,
    HeaderAppDown,
    OurHistoryApp
    
  },
  }
</script>

<style lang="css" scoped>

</style>