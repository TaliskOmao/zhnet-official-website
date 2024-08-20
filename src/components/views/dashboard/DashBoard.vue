<template>
  <div>
    <div class="text-xl mt-10">OMAO OÜ - AS59538</div>
    <div class="lg:text-7xl <lg:text-5xl leading-normal mt-6"><font color="#a233ff">Delivering</font> Internet<font color="#1bff71"> Traffic</font></div>
    <div class="text-2xl mt-20 lg:w-[50%] <lg:w-[100%]">
      <div class="leading-relaxed">
        OMAO OÜ (AS59538) operates high-performance
        <span class="font-extrabold">Network Carrier Services</span>, provides high-bandwidth
        <span class="font-extrabold">Cloud services</span>, and doing
        <span class="font-extrabold">LIR Services</span> by RIPE NCC.
      </div>
    </div>
    <div class="text-2xl mt-20">
      <a class="cursor-pointer hover:underline" @click="go('network')">About OMAO-NETS</a>
      <span class="mx-4">|</span>
      <a class="cursor-pointer hover:underline" @click="go('placeholder')"><font color="orange">Get a Quote</font></a>
      <span class="mx-4">|</span>
      <a class="cursor-pointer hover:underline" @click="go('colo')"><font color="orange">Colocation</font></a>
    </div>
  </div>
</template>

<script lang="ts" setup>
const emit = defineEmits<{
  (e: 'go', route: string): void;
}>();

const go = (route: string) => {
  emit('go', route);
};
</script>
