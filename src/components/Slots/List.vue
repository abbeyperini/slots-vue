<script setup>
  defineProps({
    listItems: Array,
  })
</script>

<template>
  <ul>
    <li v-for="listItem in listItems" :key="listItem.id">
      <slot name="item" :item="listItem"></slot>
    </li>
  </ul>
</template>