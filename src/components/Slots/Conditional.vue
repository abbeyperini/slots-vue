<template>
  <div v-if="$slots.club" class="club-container">
    <img src="../../assets/the-window.jpg" alt="the window" />
    <slot name="club"></slot>
    <img src="../../assets/the-wall.png" alt="the wall" />
  </div>
</template>