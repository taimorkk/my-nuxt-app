<template>
  <div class="mx-auto w-5/6 mb-40">
    <h1>How can Zimed® PF Help?</h1>
    <el-divider />
    <div class="help-image p-8 rounded-3xl mt-16">
      <div class="section bg-white w-1/2 h-36 my-3 rounded-2xl">
        ZIMED® PF's recommended dosage is one drop in the affected eye(s) once
        daily in the evening.
      </div>
      <div class="section bg-white w-1/2 h-36 my-3 rounded-2xl">
        ZIMED® PF is a 100% Preservative - free formula dispensed in a
        multi-dose bottle.
      </div>
      <div class="section bg-white w-1/2 h-36 my-3 rounded-2xl">
        ZIMED® PF is stored between 15 °C and 25 °C, no refrigeration needed.
      </div>
    </div>
  </div>
</template>
<script setup></script>
<style lang="scss" scoped>
h1 {
  font-size: 54px;
  font-weight: 800;
  color: #303532;
  text-align: center;
}
.el-divider {
  border-top: 3px solid #faaf1e;
  width: 30% !important;
  margin: 24px auto;
}
.help-image {
  height: 534px;
  //   background-image: url("../assets/couple.jpeg");
  background-image: linear-gradient(
      90deg,
      #f8f8f8 36.84%,
      rgba(248, 248, 248, 0) 64.47%
    ),
    url("../assets/couple.jpg");

  .section {
    padding: 1rem 4rem 1rem 2rem;
    color: #939393;
    font-size: 24px;
    font-style: normal;
    line-height: 2rem;
  }
}
</style>
