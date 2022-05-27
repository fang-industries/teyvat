<template>
  <main>
    <section id="blogs">
      <div>
        <h1 class="mb-1 text-6xl font-semibold">introductions</h1>
        <p class="mb-4 text-lg font-light text-gray-400">
          here you can see the introductions of other members of the server.
        </p>
        <div class="grid grid-cols-3 gap-8">
          <div class="rounded-lg border-2 border-dashed border-gray-600 p-4">
            <div class="flex min-h-full items-center justify-center">
              <div class="flex flex-col">
                <div class="mb-6 flex justify-center">
                  <svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="h-24 w-24 rounded-full bg-blue-300 bg-opacity-20 p-4"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                    stroke-width="2"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M12 4v16m8-8H4"
                    />
                  </svg>
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
            <div>
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
                    >(hover to reveal)</span
                  >
                </h3>
                <p
                  class="text-gray-400 blur-sm transition duration-150 hover:blur-0"
                >
                  {{ intro.details.phobias.join(', ').toLowerCase() }}
                </p>
              </div>
              <div v-if="intro.details.url">
                <a
                  :href="intro.details.url"
                  class="my-auto mt-4 flex font-medium text-blue-300 transition duration-150 hover:text-blue-200"
                  ><svg
                    xmlns="http://www.w3.org/2000/svg"
                    class="my-auto mr-2 h-5 w-5"
                    fill="none"
                    viewBox="0 0 24 24"
                    stroke="currentColor"
                    stroke-width="2"
                  >
                    <path
                      stroke-linecap="round"
                      stroke-linejoin="round"
                      d="M13.828 10.172a4 4 0 00-5.656 0l-4 4a4 4 0 105.656 5.656l1.102-1.101m-.758-4.899a4 4 0 005.656 0l4-4a4 4 0 00-5.656-5.656l-1.1 1.1"
                    /></svg
                  >link to website</a
                >
              </div>
            </div>
            <div v-for="key in intro.details"></div>
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
