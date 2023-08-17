<template>
  <div class="flex justify-center bg-white-100 min-h-screen">
    <div :class="['appContainer', 'mx-4 sm:mx-8 md:mx-auto w-full ']">
      <!-- Slot for app content -->
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AppContainer',
};
</script>
<style scoped lang="css">
.appContainer {
  max-width: 1512px;
  margin: 0 auto !important;
}
</style>
