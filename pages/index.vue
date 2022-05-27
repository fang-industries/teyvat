<template>
  <main>
    <section id="introduction">
      <div class="mb-8 flex justify-between">
        <div class="pr-8">
          <span class="text-lg font-light text-gray-400">welcome to</span>
          <h1
            class="mb-1 flex animate-gradient-x bg-gradient-to-r from-[rgb(152,198,255)] to-[rgb(219,152,255)] bg-clip-text text-6xl font-semibold leading-normal text-transparent"
          >
            <span class="hidden md:block">⁀➷&nbsp;</span>teyvat<span
              class="hidden md:block"
              >&nbsp;ˊ˗</span
            >
          </h1>
          <div class="mb-2">
            <p>
              we&apos;re a chill<span class="font-sans text-gray-400">*</span>
              discord + minecraft server where you can hang out and talk to all
              sorts of people.
            </p>
            <span class="text-xs text-gray-400"
              ><span class="font-sans text-gray-400">*</span> note: we&apos;re
              actually very chaotic</span
            >
          </div>

          <nuxt-link
            to="/about"
            class="my-auto font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >
            more about the server -></nuxt-link
          >
        </div>
        <img
          src="../assets/server-icon.jpeg"
          class="hidden h-32 rounded-full md:block"
          alt="the server icon"
        />
      </div>
    </section>
    <div class="my-8 border-b border-gray-500" />
    <section id="contact">
      <div>
        <p>want an invite to this server?</p>
        <p class="mb-4">too bad, you can't; only cool people are allowed 😎</p>
        <p class="text-sm text-gray-400">
          just kidding, contact
          <a
            href="https://discord.com/users/728180364962562108"
            class="my-auto font-medium text-[rgb(184,190,200)] underline transition duration-150 hover:text-gray-200"
            >cha <span class="font-sans">☆</span>#6171</a
          >
          or
          <a
            href="https://discord.com/users/648896419020668928"
            class="my-auto font-medium text-[rgb(184,190,200)] underline transition duration-150 hover:text-gray-200"
            >yeeeeee#1798</a
          >
          for more information.
        </p>
      </div>
    </section>
  </main>
</template>
