<template>
  <section class="flex justify-center gap-4 wrapper">
    <div class="dotedTop">
      <img src="../assets/dotedTop.png" alt="dotedTop" />
    </div>
    <div class="flex flex-col gap-4 portion">
      <h1>Free forever for your <span class="salary">salary payment</span></h1>
      <h5>Subscribe to the Eazilife today</h5>
      <div class="flex gap-16">
        <Tag
          outer-logo="./src/assets/Ellipse.svg"
          inner-logo="./src/assets/ic_baseline-apple.svg"
          title="Download on the"
          tag="AppStore"
        />
        <Tag
          outer-logo="./src/assets/Ellipse.svg"
          inner-logo="./src/assets/googleLogo.svg"
          title="Get on"
          tag="Google Play"
        />
      </div>
    </div>
    <div class="portion">
      <div class="wrapper-container">
        <div class="stacked"></div>
        <div class="stacked"></div>
        <div class="stacked-mini">
          <div class="avater">
            <img src="../assets/avater.svg" alt="avater" />
          </div>
          <h4>Adebayo Kemi</h4>
          <h6>Arts & Production Officer</h6>
          <h6>Female | Weekly</h6>
          <h4>N150,600.78</h4>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup>
import Tag from './Tag.vue';
</script>
<style scoped>
.wrapper {
  background-color: #e6a7a5;
  height: 746.994px;
  position: relative;
  align-items: center;
}
.dotedTop {
  position: absolute;
  left: 55px;
  top: 0px;
  height: 100px;
  width: 80px;
  background-size: contain;
  z-index: 20;
}
.dotedTop img {
  width: 100%;
  height: 100%;
}
.portion {
  width: 45%;
}
h1 {
  color: var(--new-styles-text-heading, #292a29);
  font-size: 56px;
  font-style: normal;
  font-weight: 500;
  line-height: 64px; /* 114.286% */
}
.salary {
  color: #ea4e4b;
}
h5 {
  color: #292a29;
  font-size: 18px;
  font-style: normal;
  font-weight: 500;
  line-height: 24px;
}
.wrapper-container {
  position: relative;
}
.stacked {
  position: absolute;
  width: 444.742px;
  height: 490.75px;
  flex-shrink: 0;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.stacked:nth-child(1) {
  background-color: inherit;
  border: 0.5px solid #ea4e4b;
  top: -20px;
  left: 53%;
}
.stacked:nth-child(2) {
  background: url('/manRejoicing.png') #ea4e4b no-repeat;
}
.stacked-mini {
  position: absolute;
  top: -200px;
  left: 20px;
  display: flex;
  width: 144.841px;
  padding: 0px 11.522px;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 8.23px;
  border-radius: 16.46px;
  border: 0.411px solid var(--new-styles-grays-gray, #dddedd);
  background: rgba(255, 255, 255, 0.8);
  box-shadow: 0px 0px 20px 0px rgba(69, 15, 14, 0.18);
  backdrop-filter: blur(50px);
}
.avater {
  width: 40px;
  height: 40px;
}
.avater image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.stacked-mini h4 {
  color: #11453b;
  font-size: 13.168px;
  font-style: normal;
  font-weight: 700;
  line-height: 19.752px;
}
.stacked-mini h6 {
  color: #515251;
  font-size: 9.876px;
  font-style: normal;
  font-weight: 400;
  line-height: 13.168px; /* 133.333% */
}
</style>
