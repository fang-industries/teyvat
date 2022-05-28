<template>
  <footer
    class="w-full bg-gray-900 bg-opacity-20 px-4 py-4 md:justify-start md:px-16 lg:px-32 xl:px-56 2xl:px-72"
  >
    <div class="flex flex-row text-blue-200">
      <div>
        <p class="my-auto cursor-default text-sm font-medium">
          made with love by pixel
        </p>
        <div
          class="my-auto cursor-default text-xs font-medium text-blue-400 md:flex"
        >
          <p>
            copyright © pix3l_ 2022<span class="hidden md:inline-block"
              >&nbsp-&nbsp;</span
            >
          </p>
          <span
            v-if="$route.path === '/licenses'"
            class="my-auto cursor-default font-medium text-white"
          >
            license notice
          </span>
          <nuxt-link
            v-if="$route.path !== '/licenses'"
            to="/licenses"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
            >license notice</nuxt-link
          >
        </div>
      </div>
    </div>
  </footer>
</template>
