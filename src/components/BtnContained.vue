<template>
  <button :class="['btnContained', custom]">
    {{ title }}
  </button>
</template>

<script>
export default {
  props: {
    title: String,
    custom: String, // Additional custom classes
  },
};
</script>

<style scoped>
.btnContained {
  font-size: 14px;
  font-size: normal;
  line-height: 500;
  line-height: 20px;
  letter-spacing: 0.1px;
  display: flex;
  width: 168px;
  padding: 10px, 32px;
  justify-content: center;
  align-items: center;
  gap: 8px;
  color: #fff;
  background: #11453b;
  box-shadow: 0px 8px 16px 0px rgba(17, 69, 59, 0.2);
  border-radius: 24px;
  border: 1px solid #11453b;
}
</style>
