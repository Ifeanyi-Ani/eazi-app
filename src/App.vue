<template>
  <div id="app">
    <AppContainer>
      <!-- Your app content goes here -->
      <router-view />
    </AppContainer>
  </div>
</template>

<script>
import AppContainer from './components/AppContainer.vue';

export default {
  components: {
    AppContainer,
  },
};
</script>
