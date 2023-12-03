<template>
  <div class="mx-auto w-5/6 administration-section mb-40">
    <div class="flex p-8 gap-10 rounded-3xl mt-16 text-center">
      <p class="info-text w-1/2">
        For more information, please see the
        <span class="p-medi"> Patient Medication Information</span> or contact
        your Health Care professional.
      </p>
      <div class="w-1/2 pl-8">
        <h2>Dosing & Administration</h2>
        <div class="section flex bg-white h-fit my-3 rounded-2xl">
          <img src="`/_nuxt/assets/drop.jpg`" class="h-16" alt="" />
          ZIMED® PF's recommended dosage is one drop in the affected eye(s) once
          daily in the evening.
        </div>
        <div class="section flex bg-white h-fit my-3 rounded-2xl">
          <img src="`/_nuxt/assets/drop.jpg`" class="h-16" alt="" />
          ZIMED® PF is a 100% Preservative - free formula dispensed in a
          multi-dose bottle.
        </div>
        <div class="section flex bg-white h-fit my-3 rounded-2xl">
          <img src="`/_nuxt/assets/drop.jpg`" class="h-16" alt="" />
          ZIMED® PF is stored between 15 °C and 25 °C, no refrigeration needed.
        </div>
      </div>
    </div>
  </div>
</template>
<script setup></script>
<style lang="scss" scoped>
.administration-section {
  h2 {
    color: #303532;
    font-size: 40px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
  }
  .info-text {
    width: 527px;
    color: #303532;
    font-size: 40px;
    font-style: normal;
    font-weight: 700;
    line-height: 145.4%;
    text-align: left;
    padding: 2rem;
    .p-medi {
      color: #01b7c4;
    }
  }
}
.section {
  padding: 1rem 2rem 1rem 2rem;
  color: #303532;
  text-align: left;
  gap: 2rem;
  font-size: 20px;
  font-style: normal;
  font-weight: 500;
  line-height: normal;
}
</style>
