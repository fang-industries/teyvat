<template>
  <nav
    class="sticky top-0 z-50 w-full bg-gray-900 bg-opacity-20 py-4 backdrop-blur-lg backdrop-filter"
  >
    <div class="mx-auto flex max-w-4xl flex-row justify-between">
      <nuxt-link
        to="/"
        class="my-auto font-semibold text-white text-blue-300 transition duration-150 hover:text-gray-200 hover:underline"
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
            v-if="$route.path !== '/'"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            home</nuxt-link
          >
        </div>
        <div>
          <p
            v-if="$route.path === '/about'"
            class="my-auto cursor-default font-medium text-white"
          >
            about
          </p>
          <nuxt-link
            to="/about"
            v-if="$route.path !== '/about'"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            about</nuxt-link
          >
        </div>
        <div>
          <p
            v-if="$route.path === '/blog'"
            class="my-auto cursor-default font-medium text-white"
          >
            blog
          </p>
          <nuxt-link
            v-if="$route.path !== '/blog'"
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
