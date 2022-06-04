<!-- ily trobo - reference: github.com/trobonox/trobo.tech/blob/main/layouts/default.vue -->

<template>
  <div
    class="flex min-h-screen flex-col justify-between bg-gray-900 font-mono selection:bg-gray-600 selection:text-blue-300"
  >
    <div class="mb-8 flex w-full flex-col text-gray-200 md:mb-16">
      <div class="sticky top-0 z-50">
        <Navbar />
        <NavbarMC v-if="$route.path.startsWith('/minecraft')" />
      </div>
      <div
        class="mx-4 mt-8 text-left md:mx-16 md:mt-16 lg:mx-32 xl:mx-56 2xl:mx-72"
      >
        <Nuxt />
      </div>
    </div>
    <Footer />
  </div>
</template>

<!-- index.vue -->
<style>
/* Transitions using the page hook */
page-enter-active,
.page-enter-active {
  animation: acrossIn 0.1s ease-out both;
}
.page-leave-active {
  animation: acrossOut 0.1s ease-in both;
}
@keyframes acrossIn {
  0% {
    transform: translate3d(0, 2%, 0);
    opacity: 0;
  }
  100% {
    transform: translate3d(0, 0, 0);
  }
}
@keyframes acrossOut {
  0% {
    transform: translate3d(0, 0, 0);
  }
  100% {
    transform: translate3d(0, 2%, 0);
    opacity: 0;
  }
}
</style>
