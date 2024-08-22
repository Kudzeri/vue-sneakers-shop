<script setup>
defineProps({
  imageUrl: String,
  title: String,
  cost: Number
})
</script>

<template>
  <div
    class="relative p-8 bg-white border border-slate-100 rounded-3xl cursor-pointer transition hover:-translate-y-2 hover:shadow-xl"
  >
    <img class="absolute top-8 left-8" src="/like-2.svg" alt="Like" />
    <img :src="imageUrl" alt="Sneakers img" />
    <p>{{ title }}</p>

    <div class="flex justify-between mt-5">
      <div class="flex flex-col">
        <span class="text-slate-400">Цена:</span>
        <span class="font-bold">{{ cost }} тг.</span>
      </div>

      <img src="/plus.svg" alt="Plus" />
    </div>
  </div>
</template>
