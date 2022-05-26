<!-- ily trobo - reference: github.com/trobonox/trobo.tech/blob/main/layouts/default.vue -->

<template>
  <div
    class="flex min-h-screen w-full flex-col justify-between bg-gray-900 font-mono text-gray-200"
  >
    <Navbar />
    <div class="mx-auto max-w-4xl px-8 pt-8">
      <Nuxt />
    </div>
    <Footer />
  </div>
</template>
