<template>
  <section class="main">
    <div class="flex flex-col justify-center items-start mt-8">
      <div class="mt-20">
        <div :class="['flex flex-col', 'wrapper']">
          <h1>
            Run your <span class="payroll">payroll </span><br />
            <span class="easily">easily</span> in
            <span class="seconds">seconds</span>
          </h1>
          <p class="text-lg">
            We’ve built an all-inclusive simple solution for <br />
            individual and businesses to manage staff, pay <br />
            salaries, bills, and relevant taxes all at once.
          </p>
          <BtnContained title="Start Using free, Forever" :custom="custom" />
        </div>
      </div>
      <div>
        <a href="#" class="text-green-700 underline">
          Download the Easipay App
        </a>
        <div class="flex gap-16 mt-4">
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
      <!-- You can add the second column content here -->
    </div>
  </section>
</template>

<script>
import BtnContained from './BtnContained.vue'; // Adjust the path
import Tag from './Tag.vue'; // Adjust the path

export default {
  components: {
    BtnContained,
    Tag,
  },
  data() {
    return {
      custom: 'your-custom-classes', // Add your custom classes here
      ellipseLogo: 'path-to-ellipse-logo.png', // Adjust the logo paths
      appleLogo: 'path-to-apple-logo.png',
      googleLogo: 'path-to-google-logo.png',
      show: 'your-show-classes', // Add your show classes here
    };
  },
};
</script>

<style scoped>
.main {
  gap: 72px;
  display: flex;
  flex-direction: column;
  width: 50%;
  justify-content: flex-start;
  align-items: center;
}
.wrapper {
  gap: 24px;
}
.wrapper h1 {
  font-weight: 700;
  font-size: 64px;
  line-height: 72px;
  color: #292a29;
}
.payroll {
  color: #11453b;
}
.easily {
  color: #b4a572;
}
.seconds {
  color: #ea4e4b;
}
</style>
