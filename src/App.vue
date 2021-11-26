<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import SpinButton from './components/SpinButton.vue';
</script>

<template>
  <SpinButton :start="0">
    <template #increment>less</template>
    <template #decrement>more</template>
  </SpinButton>
</template>
