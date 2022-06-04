<template>
  <main>
    <section id="introduction">
      <div>
        <h1 class="mb-1 text-6xl font-semibold">
          <h1 class="mb-1 text-6xl font-semibold">
            <span class="lg:hidden">faq</span
            ><span class="hidden lg:inline-block"
              >frequently asked questions</span
            >
          </h1>
        </h1>
        <p class="mb-8 text-lg font-light text-gray-400">
          have a question? make sure to check this page out!
        </p>
      </div>
    </section>
    <section id="joining">
      <p class="mb-4 text-lg font-light text-gray-400">
        how do i join the teyvat minecraft server?
      </p>
      <div>
        <p class="mb-2">
          joining the server is very easy! simply add the server IP address onto
          either the direct connect field, or add it on your Minecraft servers
          list.
        </p>
        <p class="mb-8">
          our server&apos;s IP address is >>
          <a
            href="https://mc.pnxl.dev"
            class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
            >mc.pnxl.dev</a
          >
        </p>
      </div>
    </section>
    <section id="whitelist">
      <p class="mb-4 text-lg font-light text-gray-400">
        i&apos;m not white-listed! what do i do?
      </p>
      <div>
        <p class="mb-2">currently, the server is still invite-only.</p>
        <p class="mb-8">
          for now, you&apos;ll have to contact either
          <a
            href="https://discord.com/users/728180364962562108"
            class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
            >cha <span class="font-sans">☆</span>#6171</a
          >,
          <a
            href="https://discord.com/users/648896419020668928"
            class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
            >yeeeeee#1798</a
          >
          or
          <a
            href="https://discord.com/users/967724967741513808"
            class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
            >PixelSquared#9976</a
          >
          to get white-listed.
        </p>
      </div>
    </section>
    <section id="questions">
      <p class="mb-4 text-lg font-light text-gray-400">
        have some more questions?
      </p>
      <div class="flex flex-row">
        <p>
          you might want to
          <nuxt-link
            to="/minecraft/faq"
            class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
            >read the faq</nuxt-link
          >
        </p>
        .
      </div>
    </section>
  </main>
</template>
