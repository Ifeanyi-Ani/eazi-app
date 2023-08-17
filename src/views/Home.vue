<template>
  <div class="cont-wrap">
    <Header />
    <Home_sec1 />
  </div>
  <Home_sec2 />
  <Home_sec3 />
</template>

<script>
import Header from '../components/Header.vue'; // Adjust the path based on your project structure
import Home_sec1 from '../components/Home_sec1.vue';
import Home_sec2 from '../components/Home_sec2.vue';
import Home_sec3 from '../components/Home_sec3.vue';

export default {
  components: {
    Header,
    Home_sec1,
    Home_sec2,
    Home_sec3,
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
