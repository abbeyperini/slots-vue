<script setup>
  import { ref, computed } from "vue"
  const likeCount = ref(0);
  const message = computed(() => likeCount.value < 10 ? "You love me!" : "You really love me!")
  function handleClick() {
    likeCount.value += 1;
  }
</script>
<template>
  <div class="likes-container">
    <slot :number="likeCount" :message="message"></slot>
    <!-- <h2><slot>default</slot></h2>
    <slot name="display" :number="likeCount" :message="message"></slot> -->
    <button type="button" @click.prevent="handleClick">Like</button>
  </div>
</template>