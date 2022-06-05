<template>
  <nav
    class="flex w-full flex-col bg-black bg-opacity-30 py-4 backdrop-blur-lg backdrop-filter"
  >
    <div
      class="mx-4 flex-col space-y-2 md:mx-16 md:flex-row md:justify-between md:space-y-0 lg:mx-32 xl:mx-56 2xl:mx-72"
    >
      <nuxt-link
        to="/"
        class="my-auto flex animate-gradient-x justify-center bg-gradient-to-r from-[rgb(152,198,255)] to-[rgb(219,152,255)] bg-clip-text font-sans text-transparent transition duration-150 hover:text-gray-200"
      >
        <h1 class="my-auto mr-1">⁀➷</h1>
        <h1 class="my-auto ml-1">ˊ˗</h1>
      </nuxt-link>
      <div class="flex justify-center">
        <div class="mr-8 hidden md:block">
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
        <div class="mr-6 md:mr-8">
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
        <div class="mr-6 md:mr-8">
          <p
            v-if="$route.path === '/intros' || $route.path === '/intros/'"
            class="my-auto cursor-default font-medium text-white"
          >
            intros
          </p>
          <nuxt-link
            v-else
            to="/intros"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            intros</nuxt-link
          >
        </div>
        <div class="mr-6 hidden md:mr-8 md:block">
          <p
            v-if="$route.path.startsWith('/minecraft')"
            class="my-auto cursor-default font-medium text-white"
          >
            minecraft
          </p>
          <nuxt-link
            v-else
            to="/minecraft"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            minecraft</nuxt-link
          >
        </div>
        <div class="mr-6 md:mr-8 md:hidden">
          <p
            v-if="$route.path.startsWith('/minecraft')"
            class="my-auto cursor-default font-medium text-white"
          >
            mc
          </p>
          <nuxt-link
            v-else
            to="/minecraft"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            mc</nuxt-link
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

<script>
export default {
  async asyncData({ $content, params }) {
    const articles = await $content('articles')
      .only(['slug', 'title', 'description'])
      .sortBy('createdAt', 'desc')
      .fetch()
    return {
      articles,
    }
  },
}
</script>
