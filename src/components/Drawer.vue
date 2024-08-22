<script setup>
import DrawerHead from './DrawerHead.vue'
import CartItemList from './CartItemList.vue'
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-70"></div>
  <div class="bg-white w-96 h-full fixed top-0 right-0 z-20 p-8">
    <DrawerHead />

    <CartItemList />

    <div class="flex flex-col gap-4">
      <div class="flex gap-2">
        <span>Итого:</span>
        <div class="flex-1 border-b border-dotted"></div>
        <span class="font-bold">12990 ₸</span>
      </div>

      <div class="flex gap-2">
        <span>Налог 5%:</span>
        <div class="flex-1 border-b border-dotted"></div>
        <span class="font-bold">900 ₸</span>
      </div>
    </div>
  </div>
</template>
