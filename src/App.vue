<script setup>
import { onMounted, ref } from 'vue'
import axios from 'axios'

import Header from './components/Header.vue'
import CardList from './components/CardList.vue'
import Drawer from './components/Drawer.vue'

const items = ref([])

onMounted(async () => {
  try {
    const { data } = await axios.get('https://cfd9563998ee0fec.mokky.dev/items')

    items.value = data
  } catch (e) {
    console.log(e)
  }
})
</script>

<template>
  <!-- <Drawer /> -->
  <div class="bg-white rounded-xl shadow-xl w-4/5 m-auto mt-14">
    <Header />

    <div class="p-10">
      <div class="flex justify-between items-center">
        <h2 class="text-3xl font-bold mb-8">Все кроссовки</h2>

        <div class="flex gap-4">
          <select class="py-2 px-3 border rounded-md outline-none">
            <option>По названию</option>
            <option>По цене (дешевые)</option>
            <option>По цене (дорогие)</option>
          </select>

          <div class="relative cursor-pointer">
            <img class="absolute left-4 top-3" src="/search.svg" alt="Search" />
            <input
              class="border border-slate-200 py-2 pl-12 pr-4 rounded-lg outline-none focus:border-gray-400"
              placeholder="Поиск..."
              type="text"
            />
          </div>
        </div>
      </div>

      <div class="mt-10">
        <CardList :items="items" />
      </div>
    </div>
  </div>
</template>
