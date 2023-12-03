<template>
  <BaseNavbar />
  <div class="container w-full min-w-full bg-stone-50">
    <slot />
  </div>
</template>

<script>
import BaseNavbar from "@/components/baseNavbar.vue";
export default {
  components: {
    BaseNavbar,
  },
};
</script>

<style>
.bg-primary {
  background-color: #01b7c4;
}
</style>
