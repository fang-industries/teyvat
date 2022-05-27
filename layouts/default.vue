<!-- ily trobo - reference: github.com/trobonox/trobo.tech/blob/main/layouts/default.vue -->

<template>
  <div class="flex min-h-screen flex-col justify-between bg-gray-900 font-mono">
    <div class="mb-8 flex w-full flex-col text-gray-200 md:mb-16">
      <Navbar />
      <div class="mx-4 mt-8 text-left md:mx-56 md:mt-16">
        <Nuxt />
      </div>
    </div>
    <Footer />
  </div>
</template>
