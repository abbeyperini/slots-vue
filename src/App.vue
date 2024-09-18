/*
* Default, named, and scoped slots
*/
<script setup>
import SlotsDefault from './components/Slots/Default.vue'
import SlotsNamed from './components/Slots/Named.vue'
import SlotsScoped from './components/Slots/Scoped.vue'
</script>

<template>
  <!--**Default**-->
  <SlotsDefault></SlotsDefault>
  
  <!-- <SlotsDefault>
    <span>To the Window</span>
  </SlotsDefault> -->

  <!--**Named**-->
  <!-- <SlotsNamed>
    <template #title>
      <span>To the Window</span>
    </template>
  </SlotsNamed> -->

  <!--**Named and Default**-->
  <!-- <SlotsNamed>
    <template #title>
      <span>To the Window</span>
    </template>
    <p>to</p>
    <p>The Wall</p>
  </SlotsNamed> -->

  <!-- <SlotsNamed>
    <template #title>
      <span>The Window</span>
    </template>
    <template #default>
      <p>to</p>
      <p>The Wall</p>
    </template>
  </SlotsNamed> -->

  <!--**Scoped**-->
  <!-- <SlotsScoped v-slot="slotProps">
    <h2>Shots</h2>
    <p>{{ slotProps.number }}</p>
    <p>{{ slotProps.message }}</p>
  </SlotsScoped> -->

  <!-- <SlotsScoped>
    <template #default="slotProps">
      <span>{{ slotProps.number }} Shots!</span>
    </template>
    <template #display="slotProps">
      <p>{{ slotProps.message }}</p>
    </template>
  </SlotsScoped> -->

  <!-- <SlotsScoped>
    <template #default="{ number }">
      <span>{{ number }} Shots!</span>
    </template>
  <template #display="{ message }">
      <p>{{ message }}</p>
    </template>
  </SlotsScoped> -->
</template>

/*
* Dynamic List
*/
<!-- <script setup>
  import SlotsList from './components/Slots/List.vue'
  const shotsList = [
    {
      name: "Lemon drop",
      description: "Citrusy",
      count: 2,
    },
    {
      name: "Three Wise Men",
      description: "Johnnie Walker, Jack Daniel, and Jim Beam",
      count: 3
    },
    {
      name: "Patron",
      description: "On the rocks",
      count: 4
    },
  ];
</script>
<template>
  <SlotsList :listItems="shotsList">
    <template #item="{ item }">
      <div class="shot">
        <h3>{{ item.name }}</h3>
        <p>{{ item.description }}</p>
        <span class="count">{{ item.count }}</span>
      </div>
    </template>
  </SlotsList>
</template> -->
