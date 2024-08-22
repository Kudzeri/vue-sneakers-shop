<script setup>
import Header from './components/Header.vue'
import CardList from './components/CardList.vue'
import Drawer from './components/Drawer.vue'
</script>

<template>
  <Drawer />
  <div class="bg-white rounded-xl shadow-xl w-4/5 m-auto mt-14">
    <Header />

    <CardList />
  </div>
</template>
