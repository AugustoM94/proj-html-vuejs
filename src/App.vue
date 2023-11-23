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
  <FooterAppUp/>
  <FooterAppDown/>
  <div class="scroll-to-top" @click="scrollTop">
    <i class="fas fa-chevron-up"></i>
  </div>
</template>

<script>
import '@fortawesome/fontawesome-free/css/all.css';
import HeaderAppUp from './components/HeaderAppUp.vue';
import HeaderAppDown from './components/HeaderAppdown.vue';
import OurHistoryApp from './components/OurHistoryApp.vue';
import ServicesApp from './components/ServicesApp.vue';
import ServicesDownApp from './components/ServicesDownApp.vue';
import OurYatchApp from './components/OurYatchApp.vue';
import EnjoyApp from './components/EnjoyApp.vue';
import YachtsmenApp from './components/YachtsmenApp.vue';
import TestimonialsApp from './components/TestimonialsApp.vue';
import FooterAppUp from './components/FooterAppUp.vue';
import FooterAppDown from './components/FooterAppDown.vue';
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
  TestimonialsApp,
  FooterAppUp,
  FooterAppDown
  
},
methods: {
scrollTop() {
const scrollDuration = 500;
const scrollStep = -window.scrollY / (scrollDuration / 15);
const scrollInterval = setInterval(() => {
  if (window.scrollY > 0) { 
    window.scrollBy(0, scrollStep);
  } else {
    clearInterval(scrollInterval);
  }
}, 15);
},
}
}
</script>

<style lang="css" scoped>
body {
  font-family: 'Poppins', 'sans-serif';
  background-color: var(--bg-white);
}
.scroll-to-top {
position: fixed;
bottom: 20px;
right: 20px;
cursor: pointer;
border-radius: 50%;
}

.scroll-to-top i {
color: black;
font-size: 20px;
}
</style>