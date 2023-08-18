<template>
  <div class="cardBx">
    <div class="icon"><img :src="[img]" alt="icom" /></div>
    <div class="title">{{ title }}</div>
  </div>
</template>
<script>
export default {
  props: {
    img: String,
    title: String,
  },
};
</script>
<style scoped>
.cardBx {
  display: flex;
  padding: 16px 24px;
  flex-direction: column;
  align-items: center;
  gap: 16px;
  flex: 1 0 0;
  border-radius: 24px;
  border: 1px solid #e7e8e7;
  background: #fff;
  box-shadow: 0px 9px 18px 0px rgba(170, 170, 170, 0.15);
}
.icon {
  width: 56px;
  height: 56px;
}
.icon img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center;
}
.title {
  color: #515251;
  font-size: 14px;
  font-style: normal;
  font-weight: 500;
  line-height: 16px; /* 114.286% */
  letter-spacing: 0.25px;
}
</style>
