<template>
  <main>
    <section id="introduction">
      <div class="flex justify-between">
        <div class="pr-8">
          <span class="mb-1 text-lg font-light text-gray-400">welcome to</span>
          <h1 class="mb-4 text-6xl font-semibold bg-clip-text text-transparent bg-gradient-to-r from-[rgb(152,198,255)] to-[rgb(219,152,255)] animate-gradient-x">⁀➷ teyvat ˊ˗</h1>
          <p class="mb-2">
            we&apos;re a chill discord + minecraft server where you can hang out
            and talk to all sorts of people.
          </p>
          <nuxt-link
            to="/about"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            more about the server -></nuxt-link
          >
        </div>
        <img src="../assets/server-icon.jpeg" class="h-32 rounded-full" />
      </div>
    </section>
  </main>
</template>
