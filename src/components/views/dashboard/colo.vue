<template>
    <div>
      <div class="text-4xl mt-10 title-arrow">
        <a @click="emit('back')"> <ArrowUpIcon class="arrow" /> </a>
        <font color="orange">Colo at OMAO</font>
      </div>
      <div class="text-2xl mt-5">
        <img src="@/assets/texture/beijing-colo.jpeg" width="340" height="420" align="right" />
        <font color="orange"><h1 align="center">Colo at OMAO ESTONIA</h1></font><br>
        <div><h1 align="left">OMAO NETWORK offers colocation with immediate availability. We can have you setup OMAO ESTONIA EE1 the same day you order service.<br><br></h1></div>
        <div><h1 align="left">We offer plans that range from cabinet space for a single 1U server, a full cabinet, or enough cabinet space to house tens of thousands of servers.<br><br></h1></div>
        <div><h1 align="left">Within our facilities, OMAO can provide you with a connection to the Internet from 100Mbps Ethernet up to 10 Gigabit Ethernet from ELISA EE.<br><br></h1></div>
        <font color="Green"><div><h1 align="left"><a href="https://portal.shinobu.is/" target="_blank">Open in Platform</a></h1></div></font><br>
        <div class="flex-33">
              <div class="text-center">
                <header class="box-header">
                  
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
  