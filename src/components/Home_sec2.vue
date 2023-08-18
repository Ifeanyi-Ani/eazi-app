<template>
  <section class="wrapper flex flex-col py-5">
    <SectionTitle
      title="For Individuals and Businesses"
      subtitle="Join 200+ businesses using Eazipay's easy solution."
    />
    <div class="stacked-wrap">
      <div class="stacked">
        <h2>Tamper-proof Payroll for LIfe</h2>
        <h5>Your staff payroll history is kept in one place forever.</h5>
        <h5>No more excel sheet or manual records.</h5>
        <h5>Download your payroll history anytime you need it.</h5>
      </div>
      <div class="stacked">
        <h2>All Payroll, Anytime Anywhere</h2>
        <h5>
          Wherever you are Eazipay has got you covered on ALL your Payroll
          tasks.
        </h5>
        <h5>
          Whether it is Taxes, Pension insurances HMOs, trustfunds, Eazipay
          handle all your compliamces in one place and easily, in seconds!
        </h5>
      </div>
      <div class="stacked">
        <h2>Payroll in Seconds</h2>
        <h5>Never again wil you spend more than 2 minutes on payroll.</h5>
        <h5>Just click on your staff annd bulk-pay them at once.</h5>
        <h5>Payment is done permanently.</h5>
      </div>
    </div>
    <h4>
      We are happy to answer your queries. Please, reach us at <br />
      <span>hello@myeazipay.com</span> and expect our response shortly after.
    </h4>
  </section>
</template>
<script setup>
import SectionTitle from './SectionTitle.vue';
</script>
<style scoped>
.wrapper {
  background: url('/home_sec2_bg.png');
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  align-items: center;
  gap: 64px;
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
h4 span {
  color: #ea4e4b;
}
.stacked-wrap {
  position: relative;
  width: 1128px;
  height: 320px;
  margin: auto;
}
.stacked {
  display: flex;
  width: 552px;
  height: 320px;
  padding: 64px;
  flex-direction: column;
  align-items: flex-start;
  gap: 10px;
  flex-shrink: 0;
  border-radius: 16px;
  background: radial-gradient(
      50% 50% at 50% 50%,
      rgba(217, 235, 205, 0.14) 0%,
      rgba(217, 235, 205, 0.03) 100%
    ),
    #11453b;
  box-shadow: -11px 0px 19px 0px rgba(23, 23, 23, 0.3),
    0px 13px 20px 0px rgba(23, 23, 23, 0.2);
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.stacked h2 {
  color: #fff;
  font-size: 28px;
  font-style: normal;
  font-weight: 700;
  line-height: 36px; /* 128.571% */
}
.stacked h5 {
  color: #fff;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 24px;
}
.stacked:nth-child(1) {
  left: 25%;
}
.stacked:nth-child(3) {
  left: 75%;
}
</style>
