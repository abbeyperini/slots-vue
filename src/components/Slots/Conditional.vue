<template>
  <div v-if="$slots.club" class="club-container">
    <p>The Window</p>
    <slot name="club"></slot>
    <p>The Wall</p>
  </div>
</template>