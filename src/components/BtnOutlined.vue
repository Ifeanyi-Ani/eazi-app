<template>
  <button :class="['btnOutlined', custom]">
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

<style scoped lang="css">
.btnOutlined {
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
  color: #11453b;
  border-radius: 24px;
  border: 1px solid #11453b;
}
</style>
