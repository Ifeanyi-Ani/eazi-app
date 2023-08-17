<template>
  <div class="cont-wrap">
    <Header />
    <section1 />
  </div>
  <section2 />
  <section3 />
  <section4 />
  <section5 />
  <Footer />
</template>

<script>
import Header from '../components/Header.vue'; // Adjust the path based on your project structure
import Home_sec1 from '../components/Home_sec1.vue';
import Home_sec2 from '../components/Home_sec2.vue';
import Home_sec3 from '../components/Home_sec3.vue';
import Home_sec4 from '../components/Home_sec4.vue';
import Home_sec5 from '../components/Home_sec5.vue';
import Footer from '../components/Footer.vue';

export default {
  components: {
    Header,
    section1: Home_sec1,
    section2: Home_sec2,
    section3: Home_sec3,
    section4: Home_sec4,
    section5: Home_sec5,
    Footer,
  },
};
</script>

<style scoped>
/* Add your component-specific styles here */
.cont-wrap {
  min-height: 110vh;
  margin-right: unset !important;
  background: url('./src/assets/frame.svg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center top;
  padding: unset;
}
</style>
