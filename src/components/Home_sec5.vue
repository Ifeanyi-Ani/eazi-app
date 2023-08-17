<template>
  <section class="flex justify-center gap-4 py-20 relative items-center">
    <div class="portion">
      <h1>
        Get an Exclusive <br />
        Demo of Eazipay
      </h1>
      <h5>
        Our greatest priority is to put you and your business first. Let’s show
        you how we can help.
      </h5>
    </div>
    <div class="portion flex flex-col gap-4 items-center">
      <h3>First things first</h3>
      <h6>
        We want to serve you better. Tell us a bit about yourself or company
      </h6>
      <div class="flex gap-2 border rounded-full p-3">
        <BtnContained title="Individual" />
        <BtnOutlined title="Company" />
      </div>
      <form action="" class="w-full flex flex-col gap-4 p-10">
        <div class="form-group">
          <input
            type="text"
            placeholder="First Name"
            class="appearance-none block w-full bg-white-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
          />
        </div>
        <div class="form-group">
          <input
            type="text"
            placeholder="Last Name"
            class="appearance-none block w-full bg-white-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
          />
        </div>
        <div>
          <input
            type="email"
            placeholder="Email Name"
            class="appearance-none block w-full bg-white-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
          />
        </div>
        <div class="form-group">
          <input
            type="text"
            class="appearance-none block w-full bg-white-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
            placeholder="Job title"
          />
        </div>
        <div class="form-group">
          <input
            type="number"
            class="appearance-none block w-full bg-white-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
            placeholder="Company size"
          />
        </div>
        <div class="form-group flex justify-center">
          <BtnContained title="Request Demo" />
        </div>
      </form>
    </div>
  </section>
</template>
<script setup>
import BtnContained from './BtnContained.vue';
import BtnOutlined from './BtnOutlined.vue';
</script>
<style scoped>
.portion {
  width: 45%;
}
.portion:nth-child(2) {
  border-radius: 32px;
  border: 1px solid #e7e8e7;
  background: #fff;
  box-shadow: 0px 20px 48px 0px rgba(170, 170, 170, 0.29);
}
h1 {
  color: #11453b;
  font-size: 64px;
  font-style: normal;
  font-weight: 500;
  line-height: 72px; /* 112.5% */
}
h3 {
  color: #292a29;
  text-align: center;
  font-size: 28px;
  font-style: normal;
  font-weight: 700;
  line-height: 48px;
}
h5 {
  color: #515251;
  font-size: 24px;
  font-style: normal;
  font-weight: 400;
  line-height: 32px;
}
h6 {
  color: #444;
  text-align: center;
  font-family: Aeonik;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 24px; /* 133.333% */
}
</style>
