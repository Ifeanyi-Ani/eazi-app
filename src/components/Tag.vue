<template>
  <div :class="[custom]">
    <div
      class="flex gap-12 p-3 bg-white rounded-md border border-gray-300 shadow-md"
    >
      <div class="ellipseWraper">
        <img :src="[outerLogo]" alt="ellipse" :class="['ellipse']" />
        <img :src="[innerLogo]" alt="apple" :class="['logo']" />
      </div>
      <div class="flex flex-col justify-center textt">
        <h6 class="text-lg font-semibold">
          {{ title }} <br />
          <span :class="['title']">{{ tag }}</span>
        </h6>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    outerLogo: String,
    innerLogo: String,
    title: String,
    tag: String,
    custom: String,
  },
};
</script>

<style scoped>
.ellipseWraper {
  border-radius: 50px;
  position: relative;
  width: 48px;
  height: 48px;
  flex-shrink: 0;
  margin: auto;
  background-color: #11453b;
}

.ellipse {
  width: 100%;
  height: 100%;
}

.logo {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.textt {
  font-size: 12px;
  font-style: normal;
  font-weight: 500;
  line-height: 16px;
  color: #515251;
}

.title {
  font-size: 18px;
  font-style: normal;
  font-weight: 700;
  line-height: 24px;
  color: #515251;
}
</style>
