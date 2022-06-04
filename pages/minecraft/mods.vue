<template>
  <main>
    <section id="introduction">
      <div>
        <h1 class="mb-1 text-6xl font-semibold">
          <h1 class="mb-1 text-6xl font-semibold">
            <span class="lg:hidden">mods</span
            ><span class="hidden lg:inline-block">included mods</span>
          </h1>
        </h1>
        <p class="mb-8 text-lg font-light text-gray-400">
          check out all the additions added to the server!
        </p>
      </div>
    </section>
    <section id="additions" class="space-y-8">
      <div class="space-y-4">
        <p class="text-lg font-light text-gray-400">data-packs</p>
        <div class="grid gap-4">
          <ModCard
            v-for="pack in datapacks"
            :name="pack.name"
            :desc="pack.desc"
            :url="pack.url"
          />
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const datapacks = await $content('datapacks').sortBy('name').fetch()
    return {
      datapacks,
    }
  },
}
</script>
