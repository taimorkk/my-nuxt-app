<template>
  <div class="mx-auto w-5/6 mb-40">
    <h1>How to use Zimed® PF?</h1>
    <el-divider />
    <div class="p-8 rounded-3xl mt-16">
      <div class="grid grid-cols-3 gap-4">
        <div
          v-for="(item, index) in items"
          :key="index"
          class="border p-4 step-container"
        >
          <div
            class="icon-section bg-primary mx-auto rounded-full w-28 h-28 p-6"
          >
            <img
              :src="`/_nuxt/assets/${item.icon}`"
              alt="Icon"
              class="w-14 h-14 mb-2 mx-auto"
            />
          </div>
          <!-- Icon (Replace 'path-to-icon' with the actual path to your icon) -->

          <!-- Heading -->
          <h3 class="text-lg font-semibold mb-2">{{ item.heading }}</h3>

          <!-- Content Text -->
          <p>{{ item.content }}</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import { ref } from "vue";
const items = ref([
  {
    icon: "eye-dropper.svg", // Import your icon using require
    heading: "Step 1",
    content:
      "Before putting a drop in the eye, release the first drop away from the eye to check the force needed to get only one drop out of the bottle.",
  },
  {
    icon: "washing-hands.svg",
    heading: "Step 2",
    content: " Wash your hands. Tilt your head back and look at the ceiling.",
  },
  {
    icon: "eye-svgrep.svg",
    heading: "Step 3",
    content:
      " Gently pull down the lower eyelid until there is a small pocket.",
  },
  {
    icon: "icon-softsqueeze-sides.svg",
    heading: "Step 4",
    content:
      "Turn the bottle upside down and squeeze it to release one drop into each eye that needs treatment.",
  },
  {
    icon: "eye-close.svg",
    heading: "Step 5",
    content: "Let go of the lower lid and close your eye for 30 seconds.",
  },
  {
    icon: "toilet-paper-solid.svg",
    heading: "Step 6",
    content:
      "Wipe off any excess that runs down the cheek or other skin areas.",
  },
  // Add more items as needed
]);
</script>
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
.step-container {
  text-align: center;
  width: 343px;
  height: 352px;
  padding: 2rem;
  border-radius: 20px;
  .icon-section {
    text-align: center;
  }
}
</style>
