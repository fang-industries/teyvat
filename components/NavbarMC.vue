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
            <span class="hidden md:inline-block">introduction</span
            ><span class="md:hidden">intro</span>
          </p>
          <nuxt-link
            v-else
            to="/minecraft"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            <span class="hidden md:inline-block">introduction</span
            ><span class="md:hidden">intro</span></nuxt-link
          >
        </div>
        <div>
          <p
            v-if="
              $route.path === '/minecraft/faq' ||
              $route.path === '/minecraft/faq/'
            "
            class="my-auto cursor-default font-medium text-white"
          >
            <span class="hidden md:inline-block">faq</span
            ><span class="md:hidden">faq</span>
          </p>
          <nuxt-link
            v-else
            to="/minecraft/faq"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            <span class="hidden md:inline-block">faq</span
            ><span class="md:hidden">faq</span></nuxt-link
          >
        </div>
        <div>
          <p
            v-if="
              $route.path === '/minecraft/mods' ||
              $route.path === '/minecraft/mods/'
            "
            class="my-auto cursor-default font-medium text-white"
          >
            <span class="hidden md:inline-block">mods</span
            ><span class="md:hidden">mods</span>
          </p>
          <nuxt-link
            v-else
            to="/minecraft/mods"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            <span class="hidden md:inline-block">mods</span
            ><span class="md:hidden">mods</span></nuxt-link
          >
        </div>
        <div>
          <p
            v-if="
              $route.path === '/minecraft/setup' ||
              $route.path === '/minecraft/setup/'
            "
            class="my-auto cursor-default font-medium text-white"
          >
            <span class="hidden md:inline-block">setup</span
            ><span class="md:hidden">setup</span>
          </p>
          <nuxt-link
            v-else
            to="/minecraft/setup"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            <span class="hidden md:inline-block">setup</span
            ><span class="md:hidden">setup</span></nuxt-link
          >
        </div>
      </div>
    </div>
  </nav>
</template>
