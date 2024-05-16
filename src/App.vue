<script setup>
import SlotsDefault from './components/Slots/Default.vue'
import SlotsNamed from './components/Slots/Named.vue'
import SlotsScoped from './components/Slots/Scoped.vue'
</script>

<template>
  <SlotsDefault>
    <!-- <span>My Title</span> -->
  </SlotsDefault>

  <!-- <SlotsNamed>
    <template #title>
      <span>My Title</span>
    </template>
  </SlotsNamed> -->

    <!-- <p>Put me in, coach!</p> -->
    <!-- <template #default>
      <p>Put me in, coach!</p>
    </template> -->

  <!-- <SlotsScoped v-slot="slotProps">
    <h2>Likes</h2>
    <p>{{ slotProps.number }}</p>
    <p>{{ slotProps.message }}</p>
  </SlotsScoped> -->
  <!-- <SlotsScoped>
    <template #default>
      <span>My Likes</span>
    </template>
    <template #display="{ number, message }">
      <p>{{ number }}</p>
      <p>{{ message }}</p>
    </template>
  </SlotsScoped> -->
</template>

<!-- <script setup>
  import SlotsList from './components/Slots/List.vue'
  const products = [
    {
      name: "Socks",
      description: "Luxury for your feet",
      count: 12,
    },
    {
      name: "Hat",
      description: "Wear it on your head",
      count: 8
    },
];
</script>
<template>
  <SlotsList :listItems="products">
    <template #item="{item}">
      <div class="product">
        <h3>{{ item.name }}</h3>
        <p>{{ item.description }}</p>
        <span class="count">{{ item.count }}</span>
      </div>
    </template>
  </SlotsList>
</template> -->
