<script setup>
import Card from './Card.vue'

const onClickAdd = () => {
  alert('added')
}
const onClickFavorite = () => {
  alert('favorited')
}
</script>

<template>
  <div class="p-10">
    <h2 class="text-3xl font-bold mb-8">Все кроссовки</h2>

    <div class="grid grid-cols-4 gap-5">
      <Card
        image-url="/sneakers/sneakers-1.jpg"
        title="Кроссовки Nike 1"
        :cost="12200"
        :is-added="true"
        :is-favorite="true"
        :on-click-add="onClickAdd"
        :on-click-favorite="onClickFavorite"
      />
    </div>
  </div>
</template>
