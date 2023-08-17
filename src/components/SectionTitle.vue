<template>
  <div class="flex flex-col gap-2 justify-center">
    <h1>{{ title }}</h1>
    <h4>{{ subtitle }}</h4>
  </div>
</template>
<script>
export default {
  props: {
    title: String,
    subtitle: String,
  },
};
</script>
<style scoped>
h1 {
  color: #11453b;
  text-align: center;
  font-size: 64px;
  font-style: normal;
  font-weight: 500;
  line-height: 64px; /* 100% */
}
h4 {
  color: #292a29;
  text-align: center;
  font-size: 20px;
  font-style: normal;
  font-weight: 400;
  line-height: 24px; /* 120% */
  letter-spacing: 0.2px;
}
</style>
