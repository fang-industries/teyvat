<!-- ily trobo - reference: github.com/trobonox/trobo.tech/blob/main/layouts/default.vue -->

<template>
  <div class="flex min-h-screen flex-col justify-between bg-gray-900 font-mono">
    <div class="mb-16 flex w-full flex-col text-gray-200">
      <Navbar />
      <div class="mx-56 mt-16 text-left">
        <Nuxt />
      </div>
    </div>
    <Footer />
  </div>
</template>
