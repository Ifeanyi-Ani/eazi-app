<template>
  <header class="bg-white-50">
    <div class="container mx-auto py-4 flex justify-evenly items-center">
      <div>
        <img src="../assets/eaziLogo.svg" alt="Logo" class="h-8" />
      </div>
      <nav class="space-x-8">
        <router-link to="/#" class="link">Individual</router-link>
        <router-link to="/#" class="link">Business</router-link>
        <router-link to="/#" class="link">Pricing</router-link>
        <router-link to="/#" class="link">Set your payroll</router-link>
        <router-link to="/dashboard" class="link">dashboard</router-link>
      </nav>
      <div class="space-x-2 flex gap-6">
        <BtnOutlined title="Login" />
        <BtnContained title="Register" />
      </div>
    </div>
  </header>
</template>

<script>
import BtnOutlined from './BtnOutlined.vue';
import BtnContained from './BtnContained.vue';

export default {
  components: {
    BtnOutlined,
    BtnContained,
  },
};
</script>
<style scoped lang="css">
.link {
  border-radius: 24px;
  border: 0px solid #515251;
  font-size: 16px;
  font-style: normal;
  font-weight: 500;
  line-height: 24px;
  color: #515251;
  cursor: pointer;
}
</style>
