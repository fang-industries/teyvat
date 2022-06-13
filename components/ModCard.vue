<template>
  <a
    :href="this.url"
    class="rounded-xl border-2 border-gray-500 p-4 transition duration-300 hover:bg-gray-800 hover:text-blue-300"
  >
    <div class="flex justify-between">
      <h2 class="text-xl font-semibold">
        {{ this.name }}
      </h2>
      <div class="my-auto flex flex-row items-center gap-2">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-auto w-8 p-1"
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
    <p class="text-gray-300">
      {{ this.desc }}
    </p>
  </a>
</template>

<script>
export default {
  props: {
    name: String,
    desc: String,
    url: String,
  },
}
</script>
