<script setup>
const navigation = [
  { name: 'Menu', href: '/menu-items' },
  { name: 'Special Dishes', href: '#' },
  { name: 'Contact', href: '#' }
]
</script>

<template>
  <div class="bg-white">
    <header class="inset-x-0 top-0 z-50">
      <nav class="flex items-center justify-between p-6 px-8" aria-label="Global">
        <div class="flex">
          <a href="#" class="-m-1.5 p-1.5">
            <span class="sr-only">Your Company</span>
            <img class="h-20 w-auto" src="/logo.webp" alt="" />
          </a>
        </div>

        <div class="flex justify-center gap-x-40">
          <a
            v-for="item in navigation"
            :key="item.name"
            :href="item.href"
            class="text-sm font-semibold leading-6 text-gray-900"
            >{{ item.name }}</a
          >
        </div>
        <div class="flex justify-end">
          <a href="#" class="text-sm font-semibold leading-6 text-gray-900"
            >Log in <span aria-hidden="true">&rarr;</span></a
          >
        </div>
      </nav>
    </header>

    <div class="pt-14 pb-14 px-8">
      <div class="flex items-center justify-center gap-10 py-15">
        <div class="text-center max-w-2xl">
          <h1 class="text-4xl font-bold tracking-tight text-gray-900 text-6xl">
            Best food in Astana. Delivered right to you
          </h1>
          <p class="mt-6 text-lg leading-8 text-gray-600">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
            incididunt ut labore et dolore magna aliqua.
          </p>
          <div class="mt-10 flex items-center justify-center gap-x-6">
            <a
              href="#"
              class="rounded-md bg-gray-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-gray-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
              >Menu</a
            >
            <a href="#" class="text-sm font-semibold leading-6 text-gray-900">Special dishes</a>
          </div>
        </div>
        <div class="relative">
          <img class="rounded-lg h-96" src="/about.png" alt="" />
          <img class="absolute h-40 -left-4 -bottom-4" src="/dish1.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>
