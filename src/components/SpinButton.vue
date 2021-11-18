<script setup lang="ts">
import { ref } from "vue";

defineProps<{ start: number }>();

const count = ref(0);
</script>

<template>
  <button class="btn-negative" @click="count--">
    <svg
      xmlns="http://www.w3.org/2000/svg"
      width="12"
      height="12"
      viewBox="0 0 24 24"
    >
      <path d="M0 10h24v4h-24z" />
    </svg>
  </button>

  <div class="spin-value">
    <input maxlength="3" type="text" name="" :value="count" id="" />
  </div>

  <button class="btn-positive" @click="count++">
    <svg
      xmlns="http://www.w3.org/2000/svg"
      width="12"
      height="12"
      viewBox="0 0 24 24"
    >
      <path d="M24 10h-10v-10h-4v10h-10v4h10v10h4v-10h10z" />
    </svg>
  </button>
</template>

<style scoped></style>
