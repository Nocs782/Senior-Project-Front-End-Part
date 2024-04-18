<script setup>
import favoriteCard from './favorite-main-card.vue'
</script>

<template>
  <div class="py-20">
    <div class="mx-auto max-w-7xl px-6 pb-20">
      <div class="mx-auto max-w-2xl text-center">
        <p class="mt-2 text-4xl font-bold tracking-tight text-gray-900">Our Favourites</p>
        <p class="mt-6 text-lg leading-8 text-gray-600">
          A carefully selected list of our favourite dishes which are enjoyed by the whole Astana
        </p>
      </div>
    </div>
    <div class="grid grid-cols-4 gap-4 px-20">
      <favoriteCard />
    </div>
  </div>
</template>
