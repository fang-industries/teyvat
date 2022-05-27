<template>
  <footer
    class="w-full justify-center bg-gray-900 bg-opacity-20 px-4 py-4 md:justify-start md:px-56"
  >
    <div class="flex flex-row text-blue-200">
      <div>
        <p class="my-auto cursor-default text-sm font-medium">
          made with love by pixel.
        </p>
        <p
          class="my-auto flex cursor-default text-xs font-medium text-blue-400"
        >
          copyright © pix3l_ 2022 -&nbsp;
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
          >
            license notice</nuxt-link
          >
        </p>
      </div>
    </div>
  </footer>
</template>
