<template>
    <HeaderAppUp/>
    <HeaderAppDown />
    <OurHistoryApp/>
    <ServicesApp />
    <ServicesDownApp/>
    <OurYatchApp/>
    <EnjoyApp/>
    <YachtsmenApp/>
</template>

<script>
import HeaderAppUp from './components/HeaderAppUp.vue';
import HeaderAppDown from './components/HeaderAppdown.vue';
import OurHistoryApp from './components/OurHistoryApp.vue';
import ServicesApp from './components/ServicesApp.vue';
import ServicesDownApp from './components/ServicesDownApp.vue';
import OurYatchApp from './components/OurYatchApp.vue';
import EnjoyApp from './components/EnjoyApp.vue';
import YachtsmenApp from './components/YachtsmenApp.vue';


  export default {
    name: 'App',
  components: {
    HeaderAppUp,
    HeaderAppDown,
    OurHistoryApp,
    ServicesApp,
    ServicesDownApp,
    OurYatchApp,
    EnjoyApp,
    YachtsmenApp
    
  },
  }
</script>

<style lang="css" scoped>
  body {
    font-family: 'Poppins', 'sans-serif';
    background-color: var(--bg-white);
 }
</style>