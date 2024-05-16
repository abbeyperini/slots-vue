<script setup>
  const likeCount = ref(0);
  const message = count < 10 ? "You love me!" : "You really love me!"
  function likeCount() {
    likeCount += 1;
  }
</script>
<template>
  <div class="likes-container">
    <slot :number="likeCount" :message="message"></slot>
    <button type="button" @click.prevent="handleClick">Like</button>
    <!-- <h2><slot>default</slot></h2>
    <slot name="display" :number="count" :message="counterMessage"></slot> -->
  </div>
</template>