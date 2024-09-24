/*
* Default, named, and scoped slots
*/
<script setup>
import SlotsDefault from './components/Slots/Default.vue';
import SlotsNamed from './components/Slots/Named.vue';
import SlotsScoped from './components/Slots/Scoped.vue';
import SlotsConditional from './components/Slots/Conditional.vue';
</script>

<template>
  <!--**Default**-->
  <SlotsDefault></SlotsDefault>
  
  <!-- <SlotsDefault>
    <img src="./assets/club-people.jpeg" alt="people in the club" />
  </SlotsDefault> -->

  <!--**Named**-->
  <!-- <SlotsNamed>
  </SlotsNamed> -->

  <!-- <SlotsNamed>
    <template #window>
      <img src="./assets/the-window.jpg" alt="the window" />
    </template>
    <template #wall>
      <img src="./assets/the-wall.png" alt="the wall" />
    </template>
  </SlotsNamed> -->

  <!--**Named and Default**-->
  <!-- <SlotsNamed>
    <template #window>
      <img src="./assets/the-window.jpg" alt="the window" />
    </template>
    <template #wall>
      <img src="./assets/the-wall.png" alt="the wall" />
    </template>
    <img src="./assets/club-people.jpeg" alt="people in the club" />
  </SlotsNamed> -->

  <!-- <SlotsNamed>
    <template #window>
      <img src="./assets/the-window.jpg" alt="the window" />
    </template>
    <template #wall>
      <img src="./assets/the-wall.png" alt="the wall" />
    </template>
    <template #default>
      <img src="./assets/club-people.jpeg" alt="people in the club" />
    </template>
  </SlotsNamed> -->

  <!--**Conditional**-->
  <!-- <SlotsConditional>
    <template #club v-if="false"><img src="./assets/club-people.jpeg" alt="people in the club" /></template>
  </SlotsConditional> -->

  <!--**Scoped**-->
  <!-- <SlotsScoped v-slot="slotProps">
    <h2>Shots</h2>
    <div class="flex-container">
      <p>{{ slotProps.number }}</p>
      <p>{{ slotProps.message }}</p>
    </div>
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
      id: 1,
    },
    {
      name: "Three Wise Men",
      description: "Johnnie Walker, Jack Daniel, and Jim Beam",
      count: 3,
      id: 2,
    },
    {
      name: "Patron",
      description: "On the rocks",
      count: 4,
      id: 3,
    },
  ];
</script>
<template>
  <SlotsList :listItems="shotsList">
    <template #item="{ item }">
      <div class="shots-container">
        <p class="list-heading">{{ item.name }}</p>
        <p>Description: {{ item.description }}</p>
        <p class="count">Count: {{ item.count }}</p>
      </div>
    </template>
  </SlotsList>
</template> -->
