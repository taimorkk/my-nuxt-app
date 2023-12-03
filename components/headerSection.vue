<template>
  <div class="mx-auto w-5/6 mb-40">
    <img class="" src="../assets/heading-logo.png" alt="" />
    <div class="flex w-4/5 mx-auto justify-between gap-8 my-16 pb-4">
      <el-input
        class=""
        placeholder="Drug identificaiton Number"
        v-model="idenNum"
      ></el-input>
      <button class="rounded-full px-16 py-8 bg-primary text-2xl text-white">
        Enter
      </button>
    </div>
  </div>
</template>
<script setup>
import { ref } from "vue";

const idenNum = ref("");
</script>

<style lang="scss" scoped>
::v-deep.el-input .el-input__wrapper {
  border-radius: 8rem !important;
  .el-input__inner {
    padding: 0 1.5rem !important;
    font-size: 24px !important;
  }
}
.enter-btn {
  background-color: #01b7c4;
}
</style>
