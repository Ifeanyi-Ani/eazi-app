<template>
  <div class="flex footer items-center p-3">
    <div class="wrapper flex flex-col items-center justify-center">
      <div class="logo">
        <img src="../assets/logo.svg" alt="logo" />
      </div>
      <div class="small">
        <span>Copyright © 2023 Eazipay.</span><br /><span
          >All rights reserved</span
        >
      </div>
      <div class="tag">
        <div class="img insta"></div>
        <div class="img twi"></div>
        <div class="img lin"></div>
        <div class="img fb"></div>
      </div>
    </div>
    <div class="flexLink flex justify-evenly">
      <ul>
        <h4>Product</h4>
        <li>Individual</li>
        <li>Businesses</li>
        <li>Request Demo</li>
        <li>Pricing</li>
      </ul>
      <ul>
        <h4>Legal</h4>
        <li>Privacy Policies</li>
        <li>Terms of Service</li>
      </ul>
      <ul>
        <h4>Resources</h4>
        <li>FAQs</li>
        <li>Blogs</li>
        <li>Carear</li>
        <li>Customer Stories</li>
      </ul>
      <ul>
        <h4>Contact Us</h4>
        <li>eazipay@gmail.com</li>
        <li>+234 816 878 9518</li>
      </ul>
    </div>
  </div>
</template>
<script></script>
<style scoped>
.footer {
  gap: 125px;
  border-top: 1px solid #eaeaea;
  background: #fff;
}
.wrapper {
  gap: 40px;
  flex: 1 0 0;
  width: 20%;
}
.logo img {
  width: 122px;
  height: 32px;
}
.small {
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: 20px; /* 142.857% */
  letter-spacing: 0.25px;
}
.tag {
  display: flex;
  justify-content: flex-start;
  gap: 10px;
}
.img {
  width: 40px;
  height: 40px;
}
.insta {
  background: url('/Instagram.svg');
  background-size: cover;
  background-position: center;
}
.twi {
  background: url('/Twitter.svg');
  background-size: cover;
  background-position: center;
}
.lin {
  background: url('/link.svg');
  background-size: cover;
  background-position: center;
}
.fb {
  background: url('/fbLogo.svg');
  background-size: cover;
  background-position: center;
}
.flexLink {
  width: 75%;
}
h4 {
  color: #292a29;
  font-size: 20px;
  font-style: normal;
  font-weight: 500;
  line-height: 24px;
  letter-spacing: 0.2px;
}
.flexLink li {
  color: #7c7c7c;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: 24px;
  cursor: pointer;
}
.flexLink ul {
  display: flex;
  width: 160px;
  flex-direction: column;
  align-items: flex-start;
  gap: 24px;
}
</style>
