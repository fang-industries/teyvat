<template>
  <article>
    <h1 class="mb-1 text-6xl font-semibold">{{ article.title }}</h1>
    <div class="mb-1 flex space-x-2 text-gray-500">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="my-auto h-5 w-5"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        stroke-width="2"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"
        />
      </svg>
      <span class="my-auto"
        >{{ createdAt }} &bull; {{ article.readingStats.text }}</span
      >
    </div>
    <p class="mb-8 font-light text-gray-400">
      {{ article.description }}
    </p>
    <nuxt-content
      :document="article"
      class="prose prose-invert max-w-none prose-h1:mb-2 prose-h1:text-6xl prose-h2:mb-2 prose-p:mb-2 prose-p:text-lg prose-p:text-gray-200 prose-a:text-blue-100 prose-a:underline prose-a:transition prose-a:duration-150 hover:prose-a:text-blue-200 prose-blockquote:font-normal prose-code:rounded-md prose-code:bg-gray-800 prose-code:p-1 prose-code:font-mono prose-code:font-medium prose-code:text-blue-300 prose-code:before:content-none prose-code:after:content-none prose-img:rounded-xl"
    />
  </article>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const article = await $content('articles', params.slug).fetch()
    return { article }
  },
  computed: {
    createdAt() {
      const dateparse = Date.parse(this.article.createdAt)
      const dateObject = new Date(dateparse)
      const options = { year: 'numeric', month: 'long', day: 'numeric' }
      return dateObject.toLocaleDateString('en-UK', options)
    },
  },
}
</script>
