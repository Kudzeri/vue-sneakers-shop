<script setup>
import Card from './Card.vue'
</script>

<template>
  <div class="p-10">
    <h2 class="text-3xl font-bold mb-8">Все кроссовки</h2>

    <div class="grid grid-cols-4 gap-5">
      <Card image-url="/sneakers/sneakers-1.jpg" title="Кроссовки Nike 1" cost="12200" />
      <Card image-url="/sneakers/sneakers-2.jpg" title="Кроссовки Nike 2" cost="13200" />
      <Card image-url="/sneakers/sneakers-3.jpg" title="Кроссовки Nike 3" cost="11200" />
      <Card image-url="/sneakers/sneakers-4.jpg" title="Кроссовки Nike 4" cost="123200" />
      <Card image-url="/sneakers/sneakers-5.jpg" title="Кроссовки Nike 5" cost="22200" />
      <Card image-url="/sneakers/sneakers-6.jpg" title="Кроссовки Nike 6" cost="42200" />
      <Card image-url="/sneakers/sneakers-7.jpg" title="Кроссовки Nike 7" cost="62500" />
      <Card image-url="/sneakers/sneakers-8.jpg" title="Кроссовки Nike 8" cost="92290" />
    </div>
  </div>
</template>
