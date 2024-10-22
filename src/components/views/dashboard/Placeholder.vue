<template>
  <div>
    <div class="text-5xl mt-10 title-arrow">
      <a @click="emit('back')"> <ArrowUpIcon class="arrow" /> </a>
      <font color="orange">Get connected</font>
    </div>
    <div class="text-2xl mt-20">
      <font color="orange"><h1 align="center">Join OTL (OMAO TELECOMMUNICATIONS LAN)</h1></font><br>
      <div><h1 align="center">Note: Internet speeds and prices depend on the technical capabilities at your address.<br>
      We provide up to 1000Mbps SFP+ Home Connections</h1></div><br><center><img src="@/assets/texture/black-wifi-router-with-three-antennas-table-with-tv-shelves-blurred-background_36682-364395.avif" /></center><br>
      <div><h1 align="center">Feel Free to Conveniently call in our expert technician to do it for you.</h1></div><br>
      <div class="flex-33">
            <div class="text-center">
              <header class="box-header">
                <p class="text-alternate-secondary"><a class="button button-wide button-gradient" href="tel:+1-771-220-6766" one-link-mark="yes"><i class="fas fa-envelope fa-left"></i>+1-771-220-6766</a></p>
              </header>
            </div>
          </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import ArrowUpIcon from '~icons/ant-design/arrow-up-outlined';
const emit = defineEmits<{
  (e: 'back'): void;
}>();
</script>

<style lang="less" scoped>
@arrow-size: 100px;
@x-offset: 20px;
@y-offset: 12px;
.title-arrow {
  transform: translateX(-@arrow-size - @x-offset);
  .arrow {
    width: @arrow-size;
    transform: translateY(@y-offset);
    @apply cursor-pointer;
  }
}
</style>
