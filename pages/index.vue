<template>
  <main>
    <section id="introduction">
      <div class="flex justify-between mb-8">
        <div class="pr-8">
          <span class="mb-1 text-lg font-light text-gray-400">welcome to</span>
          <h1 class="mb-1 text-6xl font-semibold leading-normal bg-clip-text text-transparent bg-gradient-to-r from-[rgb(152,198,255)] to-[rgb(219,152,255)] animate-gradient-x">⁀➷ teyvat ˊ˗</h1>
          <div class="mb-2">
            <p>
              we&apos;re a chill<span class="text-gray-400 font-sans">*</span> discord + minecraft server where you can hang out
              and talk to all sorts of people.
            </p>
            <span class="text-gray-400 text-xs"><span class="text-gray-400 font-sans">*</span> note: we&apos;re actually very chaotic</span>
          </div>

          <nuxt-link
            to="/about"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            more about the server -></nuxt-link
          >
        </div>
        <img src="../assets/server-icon.jpeg" class="h-32 rounded-full" alt="the server icon"/>
      </div>
    </section>
    <div class="border-b border-gray-500 my-8" />
    <section id="contact">
      <div>
        <p>want an invite to this server?</p>
        <p class="mb-4">too bad, you can't; only cool people are allowed 😉</p>
        <p class="text-sm text-gray-400">just kidding, contact <a href="https://discord.com/users/728180364962562108" class="underline my-auto font-medium text-[rgb(184,190,200)] transition duration-150 hover:text-gray-200">cha <span class="font-sans">☆</span>#6171</a> or <a href="https://discord.com/users/648896419020668928" class="underline my-auto font-medium text-[rgb(184,190,200)] transition duration-150 hover:text-gray-200">yeeeeee#1798</a> for more information.</p>
      </div>
    </section>
  </main>
</template>
