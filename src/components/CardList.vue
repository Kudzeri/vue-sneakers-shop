<script setup>
import Card from './Card.vue'

defineProps({
  items: Array
})

const onClickAdd = () => {
  alert('added')
}
const onClickFavorite = () => {
  alert('favorited')
}
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      v-for="item in items"
      :key="item.id"
      :image-url="item.imageUrl"
      :title="item.title"
      :cost="item.price"
      :is-added="false"
      :is-favorite="false"
      :on-click-add="onClickAdd"
      :on-click-favorite="onClickFavorite"
    />
  </div>
</template>
