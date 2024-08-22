<template>
  <header class="flex justify-between px-10 py-8 border-b border-slate-300">
    <div class="flex items-center gap-4">
      <img class="w-10" src="/logo.png" alt="Logo" />
      <div>
        <h2 class="font-bold text-xl uppercase">Vue scneakers</h2>
        <p class="text-slate-400">Магазин лучших кроссовок</p>
      </div>
    </div>

    <ul class="flex items-center gap-10">
      <li class="flex items-center gap-3 text-gray-400 hover:text-black cursor-pointer">
        <img src="/cart.svg" alt="Cart" />
        <span>32305 тг.</span>
      </li>
      <li class="flex items-center gap-3 text-gray-400 hover:text-black cursor-pointer">
        <img src="/heart.svg" alt="Heart" />
        <span>Закладки</span>
      </li>
      <li class="flex items-center gap-3 text-gray-400 hover:text-black cursor-pointer">
        <img src="/profile.svg" alt="Profile" />
        <span>Профиль</span>
      </li>
    </ul>
  </header>
</template>
