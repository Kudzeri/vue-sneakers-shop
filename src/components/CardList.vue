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
</template>
