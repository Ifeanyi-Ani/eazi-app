<template>
  <section class="py-20">
    <SectionTitle
      title="How Eazipay Works"
      subtitle="Get started in 3 simple steps."
    />
    <div class="wrapper flex justify-center gap-4">
      <div class="eclipse-container">
        <div class="eclipse-small positioning"></div>
        <div class="eclipse-smaller positioning"></div>
        <div class="eclipse-smallest positioning"></div>
        <div class="phone"></div>
      </div>
      <div class="col2"></div>
    </div>
  </section>
</template>
<script setup>
import SectionTitle from '../components/SectionTitle.vue';
</script>
<style scoped>
section {
  background-color: #fff;
}
.wrapper {
  margin-top: 150px;
}
.eclipse-container {
  position: relative;
  width: 45%;
  height: 584px;
}
.eclipse-small {
  width: 577.149px;
  height: 577.149px;
  flex-shrink: 0;
  border-radius: 577.149px;
  border: 0.187px solid #11453b;
  background: #f0f7eb;
}
.eclipse-smaller {
  width: 518.158px;
  height: 518.158px;
  flex-shrink: 0;
  border-radius: 518.158px;
  background: #d9ebcd;
}
.eclipse-smallest {
  width: 450.897px;
  height: 450.897px;
  flex-shrink: 0;
  border-radius: 450.897px;
  background: #11453b;
}
.eclipse-container .positioning,
.phone {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.phone {
  width: 347.614px;
  height: 682px;
  flex-shrink: 0;
  border-radius: 63.267px;
  background: url('/phone.gif'), lightgray;
  background-repeat: no-repeat;
  background-size: cover;
}
.col2 {
  width: 45%;
  height: 608px;
  flex-shrink: 0;
  background: url('/accountStep.png');
  background-repeat: no-repeat;
}
</style>
