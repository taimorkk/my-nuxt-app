<template>
  <div class="about-section mx-auto w-full pt-20">
    <p>
      WARNINGS AND
      <span class="bg-amber-400 px-2 text-white">PRECAUTIONS</span>
    </p>
    <el-divider class="yellow" />
    <div class="p-8 rounded-3xl mt-2">
      <div class="text-center">
        <img class="mx-auto" src="`/_nuxt/assets/footer-mouse.svg`" alt="" />
        <div class="info-section flex">
          <div class="w-1/3 ml-14 section-one">
            <h1 class="text-white">Zimed® PF</h1>
            <p class="text-white">
              Copyright © 2023 Zimed. All rights reserved
            </p>
          </div>
          <div class="w-1/6 section-two">
            <h2 class="mb-4">Company</h2>
            <p class="mb-2">For Patients</p>
            <p class="mb-2">For Doctors</p>
          </div>
          <div class="w-1/5 section-three">
            <h2 class="mb-4">Reach Us</h2>
            <p class="mb-2">
              <el-icon :size="20" class="mr-2 pt-1"><Message /></el-icon>
              <span>contact@aequuspharma.ca</span>
            </p>
            <p class="mb-2">
              <el-icon :size="20" class="mr-2"><PhoneFilled /></el-icon
              >1-833-542-2633
            </p>
            <p class="mb-2 flex">
              <el-icon :size="20" class="mr-2"><LocationFilled /></el-icon>
              <span>
                2820 - 200 Granville St. <br />
                Vancouver, <br />
                BCV6C 1S4
              </span>
            </p>
          </div>
          <div class="w-1/3 logo-section">
            <img src="`/_nuxt/assets/blue-grey.png`" alt="" />
          </div>
        </div>
      </div>
    </div>
    <el-divider class="white" />
    <div class="footer min-h-42 py-2">
      <span class="text-white">Copyrights All right reserved @Zimed</span>
    </div>
  </div>
</template>
<script setup>
import { PhoneFilled } from "@element-plus/icons-vue";
import { LocationFilled } from "@element-plus/icons-vue";
import { Message } from "@element-plus/icons-vue";
</script>

<style lang="scss" scoped>
.about-section {
  height: 727px;
  background: linear-gradient(
    180deg,
    rgba(1, 183, 196, 0) 11.25%,
    #00bdb6 100%
  );

  p {
    font-size: 54px;
    font-weight: 800;
    color: #303532;
    text-align: center;
  }
  .el-divider.yellow {
    border-top: 3px solid #faaf1e;
    width: 13% !important;
    margin: 24px auto;
  }
  .el-divider.white {
    border-top: 1px solid #fff;
    width: 85% !important;
    margin: 0px auto;
  }
  .info-section {
    margin-top: 13%;
    // background-image: url("../assets/hexagon-vector.png");
    fill: radial-gradient(
      95.35% 58.83% at 29.19% 80.76%,
      #4a7082 39%,
      #8ca4b0 61%,
      #fff 100%
    );
    div {
      height: fit-content;
    }
    background-blend-mode: color-burn;
    // mix-blend-mode: color-burn;
    p {
      text-align: left;
      color: #fff;
      font-size: 14px;
      font-style: normal;
      font-weight: 400;
      line-height: 24px; /* 171.429% */
    }
    .section-one {
      h1 {
        text-align: left;
        font-size: 48px;
        font-weight: 700;
      }
    }
    h2 {
      color: #fff;
      text-align: left;
      font-feature-settings: "salt" on, "liga" off;
      font-size: 20px;
      font-style: normal;
      font-weight: 700;
      line-height: 30px;
    }
  }
  .footer {
    background: #00bdb6;
    height: 8rem;
    span {
      margin-left: 6.5rem;
    }
  }
}
</style>
