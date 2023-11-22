<template>
    <HeaderAppUp/>
    <HeaderAppDown />
    <OurHistoryApp/>
    <ServicesApp />
    <ServicesDownApp/>
</template>

<script>
import HeaderAppUp from './components/HeaderAppUp.vue';
import HeaderAppDown from './components/HeaderAppdown.vue';
import OurHistoryApp from './components/OurHistoryApp.vue';
import ServicesApp from './components/ServicesApp.vue';
import ServicesDownApp from './components/ServicesDownApp.vue';



  export default {
    name: 'App',
  components: {
    HeaderAppUp,
    HeaderAppDown,
    OurHistoryApp,
    ServicesApp,
    ServicesDownApp
    
  },
  }
</script>

<style lang="css" scoped>
  body {
    font-family: 'Poppins', 'sans-serif';
    background-color: var(--bg-white);
 }
</style>