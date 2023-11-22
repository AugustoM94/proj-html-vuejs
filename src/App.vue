<template>
    <HeaderAppUp/>
    <HeaderAppDown />
    <OurHistoryApp/>
    <ServicesApp />
</template>

<script>

import HeaderAppUp from './components/HeaderAppUp.vue';
import HeaderAppDown from './components/HeaderAppdown.vue';
import OurHistoryApp from './components/OurHistoryApp.vue';
import ServicesApp from './components/ServicesApp.vue';



  export default {
    name: 'App',
  components: {
    HeaderAppUp,
    HeaderAppDown,
    OurHistoryApp,
    ServicesApp
    
  },
  }
</script>

<style lang="css" scoped>
  body {
    font-family: 'Poppins', 'sans-serif';
    background-color: var(--bg-white);
 }
</style>