<!-- Navbar.vue -->

<template>
  <nav class="bg-white p-8 h-24">
    <div class="container mx-auto flex justify-between items-center">
      <!-- Left side: Logo -->
      <div>
        <img src="../assets/nav-logo.png" alt="Logo" class="h-6 w-32" />
      </div>

      <!-- Center: Navigation Items -->
      <div class="right-items w-1/3 flex">
        <el-menu
          :default-active="activeIndex"
          class="el-menu-demo w-44 h-9"
          mode="horizontal"
          @select="handleSelect"
          :ellipsis="false"
        >
          <el-menu-item index="1">Patient's Access</el-menu-item>

          <el-menu-item index="3">Doctor's Access</el-menu-item>
          <el-menu-item index="4">Blogs</el-menu-item>

          <el-dropdown class="ml-2 min-w-fit">
            <span
              class="el-dropdown-link py-2 rounded-full border-2 border-black px-4"
            >
              {{ activeLang }}
              <el-icon class="el-icon--right ml-0">
                <arrow-down />
              </el-icon>
            </span>
            <template #dropdown>
              <el-dropdown-menu>
                <el-dropdown-item @click="activeLang = 'En'"
                  >English</el-dropdown-item
                >
                <el-dropdown-item @click="activeLang = 'Ur'"
                  >Urdu</el-dropdown-item
                >
              </el-dropdown-menu>
            </template>
          </el-dropdown>
        </el-menu>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from "vue";
import { ArrowDown } from "@element-plus/icons-vue";
const activeLang = ref("En");
</script>

<style scoped lang="scss">
/* Add your component-specific styles here */
/* Example switcher styles */

.el-menu-demo {
  height: 35px;
  border-bottom: none;
  .el-menu-item {
    background-color: white;
    font-size: 16px;
    font-style: normal;
    padding: 0 8px;
    &:hover,
    :focus,
    :not(.is-disabled):hover {
      background-color: white;
      color: #01b7c4 !important;
    }
    &.is-active {
      color: #01b7c4 !important;
      border-bottom-color: #01b7c4 !important;
    }
  }
  .el-icon--right {
    margin-left: 0;
  }
  .el-menu-item:not(.is-disabled):focus,
  .el-menu--horizontal .el-menu-item:not(.is-disabled):hover {
    background-color: white;
  }
}
</style>
