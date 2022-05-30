<template>
  <main>
    <section id="blogs">
      <div class="-mb-4">
        <h1 class="mb-1 text-6xl font-semibold">the teyvat times</h1>
        <p class="mb-4 text-lg font-light text-gray-400">
          every once in a while, i&apos;ll write about server updates to the
          minecraft, or discord server if there&apos;s any updates from the
          administrators.
        </p>
        <nuxt-link
          v-for="article in articles"
          :to="'/blog/' + article.slug"
          :key="article.title"
        >
          <div
            class="mb-4 rounded-lg border-2 border-gray-600 p-4 transition duration-150 hover:bg-gray-800 hover:text-blue-300"
          >
            <div class="flex w-full flex-row justify-between">
              <h3 class="text-xl font-semibold tracking-tight text-gray-200">
                {{ article.title }}
              </h3>
              <div class="flex flex-row items-center gap-2">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-auto w-8 rounded-md p-1"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M17 8l4 4m0 0l-4 4m4-4H3"
                  />
                </svg>
              </div>
            </div>
            <h4 class="text-gray-400">{{ article.description }}</h4>
          </div>
        </nuxt-link>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const articles = await $content('articles')
      .only(['slug', 'title', 'description', 'tags'])
      .sortBy('createdAt', 'desc')
      .fetch()
    return {
      articles,
    }
  },
}
</script>
