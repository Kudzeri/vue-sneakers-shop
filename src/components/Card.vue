<script setup>
defineProps({
  imageUrl: String,
  title: String,
  cost: Number,
  isFavorite: Boolean,
  isAdded: Boolean,
  onClickAdd: Function,
  onClickFavorite: Function
})
</script>

<template>
  <div
    class="relative p-8 bg-white border border-slate-100 rounded-3xl cursor-pointer transition hover:-translate-y-2 hover:shadow-xl"
  >
    <img
      class="absolute top-8 left-8"
      :src="isFavorite ? '/like-2.svg' : '/like-1.svg'"
      alt="Like"
      @click="onClickFavorite"
    />
    <img :src="imageUrl" alt="Sneakers img" />
    <p>{{ title }}</p>

    <div class="flex justify-between mt-5">
      <div class="flex flex-col">
        <span class="text-slate-400">Цена:</span>
        <span class="font-bold">{{ cost }} ₸</span>
      </div>

      <img
        :src="isAdded ? '/checked.svg' : '/plus.svg'"
        :alt="isAdded ? 'Checked' : 'Plus'"
        @click="onClickAdd"
      />
    </div>
  </div>
</template>
