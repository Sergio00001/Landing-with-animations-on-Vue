<template>
  <Header />
  <AboutUs />
  <OurServices />
  <Footer />
</template>
<script>
import Header from '@/components/Header'
import AboutUs from '@/components/AboutUs'
import OurServices from '@/components/OurServices'
import Footer from '@/components/Footer'
import AOS from 'aos';

import 'animate.css';
import 'aos/dist/aos.css';

export default {
  components: { Header, AboutUs, OurServices, Footer },

  mounted() {
    AOS.init();
  }
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');
@import url('@/assets/Fonts/Aileron-Regular/style.css');
@import url('@/assets/Fonts/Aileron-Bold/style.css');


* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: 'Poppins', 'Aileron', sans-serif;
}

html body {
  width: 100%;
  height: 100%;
  overflow-x: hidden;
}

#app {
  width: 100%;
  height: 100%;
}

a {
  text-decoration: none;
}

ul li {
  list-style-type: none;
}
</style>
