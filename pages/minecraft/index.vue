<template>
  <main>
    <section id="introduction">
      <div>
        <h1 class="mb-1 text-6xl font-semibold">
          <span class="md:hidden">mc</span
          ><span class="hidden md:inline-block">minecraft</span> server
        </h1>
        <p class="mb-4 text-lg font-light text-gray-400">
          find out more information about our invite-only minecraft server here!
        </p>
        <p class="mb-4">
          the teyvat minecraft server features a unique experience, featuring a
          custom world generation with Terralith, Incendium, and Nullscape, and
          contains 28 addtional data-packs, 32 mods, aswell as a custom resource
          pack.
        </p>
        <p class="mb-8">
          on top of that, the server also runs a mod loader with very low
          overhead, the bleeding-edge Quilt Project. the mod loader is based on
          the ever popular Fabric Loader, meaning compatibility is available for
          existing Fabric mods.
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
