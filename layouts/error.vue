<template>
  <main>
    <section id="introduction">
      <div class="flex justify-between">
        <div class="pr-8">
          <span class="mb-1 text-lg font-light text-gray-400">whoopsies!</span>
          <h1 class="mb-1 text-6xl font-semibold" v-if="error.statusCode === 404">that page doesn&apos;t exist!</h1>
          <h1 class="mb-1 text-6xl font-semibold" v-else>an error occured!</h1>
          <div class="mb-2">
            <p>
              how did you even get here? you should probably go back to the home page.
            </p>
          </div>
          <nuxt-link
            to="/"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            &lt;- go back home</nuxt-link
          >
        </div>
      </div>
    </section>
  </main>
</template>

<script>
  export default {
    props: ['error'],
  }
</script>
