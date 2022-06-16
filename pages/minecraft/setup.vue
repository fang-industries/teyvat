<template>
  <main>
    <section id="introduction">
      <div>
        <h1 class="mb-1 text-6xl font-semibold">
          <h1 class="mb-1 hidden text-6xl font-semibold md:block">
            setting up the game
          </h1>
          <h1 class="mb-1 text-6xl font-semibold md:hidden">launcher setup</h1>
        </h1>
        <p class="mb-8 text-lg font-light text-gray-400">
          here's how to setup your game with Quilt modloader
        </p>
      </div>
    </section>
    <section id="table-of-contents" class="mb-16 space-y-4">
      <p class="text-lg font-light text-gray-400">i want to use Quilt ...</p>
      <div class="flex flex-col space-y-2">
        <a
          href="#minecraft-launcher"
          class="font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >... with Minecraft Launcher</a
        >
        <a
          href="#multimc"
          class="font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >... with MultiMC/UltimMC</a
        >
        <a
          href="#tlauncher"
          class="font-medium text-blue-300 transition duration-150 hover:text-blue-200"
          >... with TLauncher</a
        >
      </div>
    </section>
    <section id="minecraft-launcher" class="mb-16 space-y-4">
      <p class="text-lg font-light text-gray-400">Minecraft Launcher</p>
      <div class="space-y-2">
        <p>
          installing Quilt for the vanilla Minecraft launcher is easy. before we
          start, make sure you have the following.
        </p>
        <br />
        <p class="font-light text-gray-400">pre-requisites</p>
        <ol class="ml-6 list-disc">
          <li>
            <a
              href="https://minecraft.net/download"
              class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
              >the vanilla, Minecraft Launcher</a
            >
          </li>
          <li>
            <a
              href="https://adoptium.net/"
              class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
              >Adoptium's OpenJRE 17 runtime</a
            >
          </li>
        </ol>
        <br />
        <p class="font-light text-gray-400">installation</p>
        <p>
          first, you should at least start Minecraft 1.19 once, to make sure
          that you've downloaded all needed files for Quilt to patch.
        </p>
        <p>
          then, go ahead and download the Quilt installer, which can be found
          <a
            href="https://maven.quiltmc.org/repository/release/org/quiltmc/quilt-installer/latest/quilt-installer-latest.jar"
            class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
            >here</a
          >.
        </p>
        <p>after downloading the installer, run it.</p>
        <div class="md:flex md:flex-row">
          <div class="my-auto space-y-4">
            <p>then, you'll see a window similar to this open.</p>
            <p>leave everything as default and simply press install.</p>
          </div>
          <img src="https://i.imgur.com/sCqCym4.png" alt="installer window " />
        </div>
        <p>
          now, open the Minecraft launcher and you should see a new profile
          named <span class="font-semibold">quilt-loader-1.19</span>.
        </p>
        <p>
          if that's the case, congratulations! you've sucessfully installed
          Quilt onto Minecraft.
        </p>
      </div>
    </section>
    <section id="multimc" class="mb-8 space-y-4">
      <p class="text-lg font-light text-gray-400">Minecraft Launcher</p>
      <div class="space-y-2">
        <p>
          installing Quilt for the vanilla Minecraft launcher is easy. before we
          start, make sure you have the following.
        </p>
        <br />
        <p class="font-light text-gray-400">pre-requisites</p>
        <ol class="ml-6 list-disc">
          <li>
            <a
              href="https://minecraft.net/download"
              class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
              >the vanilla, Minecraft Launcher</a
            >
          </li>
          <li>
            <a
              href="https://adoptium.net/"
              class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
              >Adoptium's OpenJRE 17 runtime</a
            >
          </li>
        </ol>
        <br />
        <p class="font-light text-gray-400">installation</p>
        <p>
          first, you should at least start Minecraft 1.19 once, to make sure
          that you've downloaded all needed files for Quilt to patch.
        </p>
        <p>
          then, go ahead and download the Quilt installer, which can be found
          <a
            href="https://maven.quiltmc.org/repository/release/org/quiltmc/quilt-installer/latest/quilt-installer-latest.jar"
            class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
            >here</a
          >.
        </p>
        <p>after downloading the installer, run it.</p>
        <div class="md:flex md:flex-row">
          <div class="my-auto space-y-4">
            <p>then, you'll see a window similar to this open.</p>
            <p>leave everything as default and simply press install.</p>
          </div>
          <img src="https://i.imgur.com/sCqCym4.png" alt="installer window " />
        </div>
        <p>
          now, open the Minecraft launcher and you should see a new profile
          named <span class="font-semibold">quilt-loader-1.19</span>.
        </p>
        <p>
          if that's the case, congratulations! you've sucessfully installed
          Quilt onto Minecraft.
        </p>
      </div>
    </section>
  </main>
</template>
