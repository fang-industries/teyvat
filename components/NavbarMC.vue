<template>
  <nav
    class="flex w-full flex-col bg-black bg-opacity-20 py-2 text-sm backdrop-blur-lg backdrop-filter"
  >
    <div
      class="mx-4 flex justify-center md:mx-16 md:justify-end lg:mx-32 xl:mx-56 2xl:mx-72"
    >
      <div class="flex space-x-8">
        <div>
          <p
            v-if="$route.path === '/minecraft' || $route.path === '/minecraft/'"
            class="my-auto cursor-default font-medium text-white"
          >
            introduction
          </p>
          <nuxt-link
            v-else
            to="/minecraft"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            introduction</nuxt-link
          >
        </div>
      </div>
    </div>
  </nav>
</template>
