<template>
  <main>
    <section id="blogs">
      <div>
        <h1 class="mb-1 hidden text-6xl font-semibold md:block">
          introductions
        </h1>
        <h1 class="mb-1 text-6xl font-semibold md:hidden">intros</h1>
        <p class="mb-4 text-lg font-light text-gray-400">
          here you can see the introductions of other members of the server.
        </p>
        <div class="grid gap-6 md:grid-cols-2 lg:grid-cols-3 2xl:grid-cols-4">
          <div
            class="rounded-lg border-2 border-dashed border-gray-600 p-4 transition duration-150 hover:border-blue-300"
          >
            <div class="flex min-h-full items-center justify-center">
              <div class="flex flex-col">
                <div class="mb-6 flex justify-center">
                  <font-awesome-icon
                    icon="fa-solid fa-plus"
                    class="rounded-full bg-blue-300 bg-opacity-20 p-7 text-[3rem]"
                  />
                </div>
                <p>this could be you!</p>
              </div>
            </div>
          </div>
          <div
            v-for="intro in intros"
            class="rounded-lg border-2 border-gray-600 p-4"
          >
            <div class="mb-2 flex">
              <img
                :src="intro.user.pfp"
                alt="avatar"
                class="my-auto mr-2 h-6 w-6 rounded-full"
              />
              <a
                :href="'https://discord.com/users/' + intro.user.id"
                class="my-auto font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
              >
                {{ intro.user.tag }}</a
              >
            </div>
            <h2 class="mb-2 text-xl font-semibold tracking-tight text-gray-200">
              {{ intro.greet }}
            </h2>
            <div class="space-y-2">
              <div class="grid grid-cols-2">
                <div v-if="intro.details.age">
                  <h3 class="text-lg">age</h3>
                  <p class="text-gray-400">
                    {{ intro.details.age.toString() }}
                  </p>
                </div>
                <div v-if="intro.details.pronouns">
                  <h3 class="text-lg">pronouns</h3>
                  <p class="text-gray-400">
                    {{ intro.details.pronouns.toLowerCase() }}
                  </p>
                </div>
              </div>
              <div v-if="intro.details.kins">
                <h3 class="text-lg">kins</h3>
                <p class="text-gray-400">
                  {{ intro.details.kins.join(', ').toLowerCase() }}
                </p>
              </div>
              <div v-if="intro.details.phobias">
                <h3 class="text-lg">
                  phobias&nbsp;<span
                    class="text-sm tracking-tight text-gray-500"
                    >(hover/tap to reveal)</span
                  >
                </h3>
                <p
                  class="text-gray-400 blur-sm transition duration-150 hover:blur-0"
                >
                  {{ intro.details.phobias.join(', ').toLowerCase() }}
                </p>
              </div>
              <div v-if="intro.socials" class="space-y-1">
                <h3 class="text-lg">links</h3>
                <div v-if="intro.socials.url">
                  <a
                    :href="'https://' + intro.socials.url"
                    class="my-auto flex font-medium text-blue-300 transition duration-150 hover:text-blue-200"
                  >
                    <font-awesome-icon
                      icon="fa-solid fa-link"
                      class="my-auto mr-2 h-5 w-5"
                    />{{ intro.socials.url }}</a
                  >
                </div>
                <div v-if="intro.socials.yt">
                  <a
                    :href="
                      'https://www.youtube.com/channel/' + intro.socials.yt[1]
                    "
                    class="my-auto flex font-medium text-blue-300 transition duration-150 hover:text-blue-200"
                  >
                    <font-awesome-icon
                      icon="fa-brands fa-youtube"
                      class="my-auto mr-2 h-5 w-5"
                    />{{ intro.socials.yt[0] }}</a
                  >
                </div>
                <div v-if="intro.socials.ig">
                  <a
                    :href="'https://www.instagram.com/' + intro.socials.ig"
                    class="my-auto flex font-medium text-blue-300 transition duration-150 hover:text-blue-200"
                  >
                    <font-awesome-icon
                      icon="fa-brands fa-instagram"
                      class="my-auto mr-2 h-5 w-5"
                    />{{ intro.socials.ig }}</a
                  >
                </div>
                <div v-if="intro.socials.twt">
                  <a
                    :href="'https://www.twitter.com/' + intro.socials.twt"
                    class="my-auto flex font-medium text-blue-300 transition duration-150 hover:text-blue-200"
                  >
                    <font-awesome-icon
                      icon="fa-brands fa-twitter"
                      class="my-auto mr-2 h-5 w-5"
                    />{{ intro.socials.twt }}</a
                  >
                </div>
                <div v-if="intro.socials.tiktok">
                  <a
                    :href="'https://www.tiktok.com/@' + intro.socials.tiktok"
                    class="my-auto flex font-medium text-blue-300 transition duration-150 hover:text-blue-200"
                  >
                    <font-awesome-icon
                      icon="fa-brands fa-tiktok"
                      class="my-auto mr-2 h-5 w-5"
                    />@{{ intro.socials.tiktok }}</a
                  >
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  async asyncData({ $content, params }) {
    const intros = await $content('intros').sortBy('createdAt', 'desc').fetch()
    return {
      intros,
    }
  },
}
</script>
