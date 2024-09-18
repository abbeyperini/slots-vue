<script setup>
  import { ref, computed } from "vue"
  const shotCount = ref(0);
  const message = computed(() => shotCount.value < 5 ? "Cups in the air!" : "Put your hands in the air!")
  function handleClick() {
    shotCount.value += 1;
  }
</script>
<template>
  <div class="shots-container">
    <slot :number="shotCount" :message="message"></slot>
    <!-- <h2><slot :number="shotCount">default</slot></h2>
    <slot name="display" :message="message"></slot> -->
    <button type="button" @click.prevent="handleClick">Take shot</button>
  </div>
</template>