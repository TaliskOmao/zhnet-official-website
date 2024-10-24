<template>
  <div>
    <div class="text-xl mt-10">OMAO OÜ - TALLINN LOCAL NETWORKS</div>
    <div class="lg:text-7xl <lg:text-5xl leading-normal mt-6"><font color="blue">Delivering</font> Internet<font color="yellow"> Traffic</font></div>
    <div class="text-2xl mt-20 lg:w-[50%] <lg:w-[100%]">
      <div class="leading-relaxed">
        <span class="font-extrabold">OMAO TELECOMMUNICATIONS LAN (OTL)</span> operates high-performance
        <span class="font-extrabold">Network Carrier Services</span>, provides high-bandwidth
        <span class="font-extrabold">Home Wireless</span>, and provide performance
        <span class="font-extrabold">CDN Services</span> from our platforms.
      </div>
    </div>
    <div class="text-2xl mt-20">
      <a class="cursor-pointer hover:underline" @click="go('network')">About OMAO-NETS</a>
      <span class="mx-4">|</span>
      <a class="cursor-pointer hover:underline" @click="go('placeholder')"><font color="orange">Get Connected</font></a>
      <span class="mx-4">|</span>
      <a class="cursor-pointer hover:underline" @click="go('colo')"><font color="orange">Business Solutions</font></a>
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
