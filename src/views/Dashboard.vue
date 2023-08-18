<template>
  <div class="wrapper w-full relative">
    <div class="side-nav fixed flex flex-col justify-start items-center">
      <div class="logo">
        <router-link to="/" class="flex justify-center items-center">
          <img src="../assets/whiteLogo.svg" alt="eazi-logo" />
        </router-link>
      </div>
      <div class="relative ul">
        <ul class="absolute w-full flex flex-col">
          <li class="active">
            <router-link to="/dashboard"
              ><span class="imgCon"
                ><img src="../assets/icon1.svg" alt="icon" /></span
              ><span class="nameCon">Dashboard</span></router-link
            >
          </li>
          <li>
            <router-link to="#"
              ><span class="imgCon"
                ><img src="../assets/icon2.svg" alt="icon" /></span
              ><span class="nameCon">Wallet</span></router-link
            >
          </li>
          <li>
            <router-link to="#"
              ><span class="imgCon"
                ><img src="../assets/icon3.svg" alt="icon" /></span
              ><span class="nameCon">Employee Management</span></router-link
            >
          </li>
          <li>
            <router-link to="#"
              ><span class="imgCon"
                ><img src="../assets/icon4.svg" alt="icon" /></span
              ><span class="nameCon">Payroll</span></router-link
            >
          </li>
          <li>
            <router-link to="#"
              ><span class="imgCon"
                ><img src="../assets/icon8.svg" alt="icon" /></span
              ><span class="nameCon">Compliance</span></router-link
            >
          </li>
          <li>
            <router-link to="#"
              ><span class="imgCon"
                ><img src="../assets/icon6.svg" alt="icon" /></span
              ><span class="nameCon">Quick Loan</span></router-link
            >
          </li>
          <li>
            <router-link to="#"
              ><span class="imgCon"
                ><img src="../assets/icon8.svg" alt="icon" /></span
              ><span class="nameCon">Book Keeping</span></router-link
            >
          </li>
          <li>
            <router-link to="#"
              ><span class="imgCon"
                ><img src="../assets/icon7.svg" alt="icon" /></span
              ><span class="nameCon">Support</span></router-link
            >
          </li>
          <li>
            <router-link to="#"
              ><span class="imgCon"
                ><img src="../assets/icon9.svg" alt="icon" /></span
              ><span class="nameCon">Support</span></router-link
            >
          </li>
        </ul>
      </div>
    </div>
    <div class="main">
      <div class="topNav flex justify-between w-full">
        <div class="companyLogo">
          <img src="../assets/companyLogo.png" alt="logo" />
        </div>
        <div class="account flex items-center gap-6">
          <div class="notification">
            <img src="../assets/notification.svg" alt="logo" />
          </div>
          <div class="actx flex items-center justify-center gap-3">
            <div class="imgCon">
              <img src="../assets/account.svg" alt="account-pics" />
            </div>
            <div class="nameCon">
              <h4>Kalu Abasiama</h4>
              <h6>Admin</h6>
            </div>
          </div>
        </div>
      </div>

      <div class="inner-container">
        <section>
          <h2>Welcome Abasiama</h2>
          <h6>Pay and manage your employee in minutes</h6>

          <div class="flexBox flex gap-10 mt-20">
            <div class="flexBx flex flex-col gap-10 w-full">
              <div class="wallet-bal flex items-center justify-between px-20">
                <div class="bal">
                  <h6>Wallet Balance</h6>
                  <h2>N12,560,078.00</h2>
                  <!-- <div class="eye"></div> -->
                </div>
                <div class="fund">
                  <button>Fund Wallet</button>
                </div>
              </div>
              <div class="actions flex justify-between gap-10">
                <CardBox />
                <CardBox />
                <CardBox />
                <CardBox />
              </div>
            </div>
            <div class="small-side">
              <div class="title"><h6 class="">Next Payroll</h6></div>
              <div class="date">
                <div class="bx"></div>
                <h6>09/11/2022</h6>
              </div>
              <div class="info">
                <h6>Total Employee</h6>
                <h2>64</h2>
              </div>
            </div>
          </div>
        </section>
      </div>
    </div>
  </div>
</template>
<script>
import CardBox from '../components/CardBox.vue';
export default {
  components: {
    CardBox,
  },
};
</script>
<style scoped>
.side-nav {
  width: 272px;
  height: 1024px;
  gap: 21.298px;
  flex-shrink: 0;
  background: #fff;
  box-shadow: 4px 0px 25px 0px rgba(170, 170, 170, 0.08);
  overflow: hidden;
}
.logo {
  width: 318.282px;
  height: 150.702px;
  flex-shrink: 0;
  background: url('./src/assets/maskLogo.svg') rgba(17, 69, 59, 0.7) no-repeat;
  background-size: cover;
}
.logo a {
  width: 100%;
  height: 100%;
}
.logo img {
  object-fit: contain;
  width: 150px;
  height: 100%;
}
.side-nav .ul {
  width: 272px;
  height: 852px;
  flex-shrink: 0;
}
.side-nav li {
  position: relative;
  border-bottom: 1px solid #e7e8e7;
  background: #fff;
  width: 272px;
  height: 56px;
}
.side-nav li.active {
  background: rgba(240, 247, 235, 0.5);
  border-bottom: #e7e8e7;
}
.side-nav li a {
  display: block;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  padding-left: 35px;
  gap: 20px;
}
.side-nav li .imgCon {
  display: block;
  width: 19.995px;
  height: 20px;
}
.side-nav li .nameCon {
  display: block;
  color: #11453b;
  font-size: 16px;
  font-style: normal;
  font-weight: 500;
  line-height: 24px; /* 150% */
}
.main {
  position: absolute;
  width: calc(100% - 272px);
  left: 272px;
  min-height: 100vh;
  background: #f9fafc;
  overflow: hidden;
}
.topNav {
  height: 80px;
  background: #fff;
  box-shadow: 0px 4px 25px 0px rgba(0, 0, 0, 0.05);
  padding: 11px 48px 11px 61px;
}
.notification img {
  width: 16px;
  height: 19.951px;
}
.actx img {
  border-radius: 56px;
  width: 56px;
  height: 56px;
}
.actx h4 {
  color: #2b2b2b;
  font-size: 16px;
  font-style: normal;
  font-weight: 700;
  line-height: 24px; /* 150% */
}
.actx h6 {
  color: #898989;
  font-size: 14px;
  font-style: normal;
  font-weight: 500;
  line-height: 16px;
  letter-spacing: 0.25px;
}
section h2 {
  color: #292a29;
  font-size: 36px;
  font-style: normal;
  font-weight: 700;
  line-height: 48px;
}
section h6 {
  color: #515251;
  font-size: 16px;
  font-style: normal;
  font-weight: 500;
  line-height: 24px;
}
.inner-container {
  width: 90%;
  margin: 50px auto;
}
.wallet-bal {
  width: 100%;
  height: 160px;
  flex-shrink: 0;
  background: url('./src/assets/maskLogo.svg') rgba(17, 69, 59, 0.7) no-repeat;
  background-size: cover;
  background-position: center;
  border-radius: 20px;
  position: relative;
}
.bal h2 {
  color: #fff;
}
.bal h6 {
  color: rgba(192, 235, 164, 0.7);
}
.fund button {
  background-color: rgba(217, 235, 205, 0.7);

  display: flex;
  align-items: center;
  justify-content: center;
  padding: 10px 18px;
  width: 150px;
  height: 56px;
  border-radius: 56px;
}
.small-side {
  border-radius: 24px;
  border: 1px solid #e7e8e7;
  background: #fff;
  box-shadow: 0px 6px 12px 0px rgba(170, 170, 170, 0.11);
  display: flex;
  width: 20%;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  align-self: stretch;
}
.title {
  display: flex;
  padding: 8px 6px;
  justify-content: center;
  align-items: center;
  gap: 10px;
  align-self: stretch;
  border-radius: 16px 16px 0px 0px;
  background: #d9ebcd;
  width: 100%;
  box-shadow: 0px 9px 18px 0px rgba(170, 170, 170, 0.15);
}
.date {
  display: flex;
  height: 89px;
  padding: 16px 6px;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 8px;
  align-self: stretch;
}
</style>
