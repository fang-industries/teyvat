<template>
  <nav
    class="sticky top-0 z-50 flex w-full flex-col bg-opacity-0 pb-4 backdrop-blur-lg backdrop-filter"
  >
    <p
      class="mb-4 bg-blue-900 bg-opacity-20 pb-2 pt-2 text-center text-sm italic"
    >
      this website is under construction! some pages may be missing, and the
      whole site might look odd on certain devices. please be patient!
    </p>
    <div class="mx-56 flex flex-row justify-between">
      <nuxt-link
        to="/"
        class="my-auto font-semibold text-blue-300 transition duration-150 hover:text-gray-200 hover:underline"
      >
        <img src="../../assets/logo.svg" class="my-auto h-4" />
      </nuxt-link>
      <div class="flex space-x-8">
        <div>
          <p
            v-if="$route.path === '/'"
            class="my-auto cursor-default font-medium text-white"
          >
            home
          </p>
          <nuxt-link
            to="/"
            v-else
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            home</nuxt-link
          >
        </div>
        <div>
          <p
            v-if="$route.path === '/about' || $route.path === '/about/'"
            class="my-auto cursor-default font-medium text-white"
          >
            about
          </p>
          <nuxt-link
            to="/about"
            v-else
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            about</nuxt-link
          >
        </div>
        <div>
          <p
            v-if="$route.path === '/blog' || $route.path === '/blog/'"
            class="my-auto cursor-default font-medium text-white"
          >
            blog
          </p>
          <nuxt-link
            v-else
            to="/blog"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            blog</nuxt-link
          >
        </div>
      </div>
    </div>
  </nav>
</template>
