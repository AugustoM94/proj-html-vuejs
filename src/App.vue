<template>
    <HeaderAppUp/>
    <HeaderAppDown />
    <OurHistoryApp/>
    <ServicesApp />
    <ServicesDownApp/>
    <OurYatchApp/>
    <EnjoyApp/>
    <YachtsmenApp/>
    <TestimonialsApp/> 
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
import TestimonialsApp from './components/TestimonialsApp.vue';


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
    YachtsmenApp,
    TestimonialsApp
    
  },
  }
</script>

<style lang="css" scoped>
  body {
    font-family: 'Poppins', 'sans-serif';
    background-color: var(--bg-white);
 }
</style>