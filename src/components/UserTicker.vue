<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****7722 生成了写给母亲六十大寿的温情感恩家书"
  },
  {
    "text": "用户 189****3311 获得了吵架后给妻子诚恳道歉手写信模板"
  },
  {
    "text": "用户 131****5599 完成了毕业十周年致高中班主任的感恩信"
  },
  {
    "text": "用户 156****4411 生成了写给考研挫折中女儿的理解鼓励信"
  },
  {
    "text": "用户 173****8800 取得了远赴重洋对挚友的寄怀信件"
  }
]);
</script>
