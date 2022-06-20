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
    <section id="table-of-contents" class="mb-16 space-y-8">
      <div class="space-y-4">
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
        <p class="font-light text-gray-400">Quilt installation</p>
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
          <img
            src="https://raw.githubusercontent.com/pnxl/teyvat/master/assets/blog/images/quilt-setup/Screenshot%202022-06-16%20at%2016.07.26.png"
            alt="installer window"
          />
        </div>
        <p>
          now, open the Minecraft launcher and you should see a new profile
          named
          <span class="font-semibold italic">quilt-loader-1.19</span>.
        </p>
        <p>
          if that's the case, congratulations! you've sucessfully installed
          Quilt onto Minecraft.
        </p>
        <br />
        <p class="font-light text-gray-400">mod installation</p>
        <p>
          start by downloading the modpack, which can be found
          <!-- TODO: add link -->
          <a
            href="PLACEHOLDER LINK FOR MODPACK"
            class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
            >here</a
          >.
        </p>
        <p>
          extract the contents of the ZIP file you downloaded, preferrably onto
          a folder to keep your files from being messy.
        </p>
        <p>
          now, click on the Installations tab on the Minecraft launcher, hover
          over your Quilt profile and click on the folder icon.
        </p>
        <div class="flex flex-row justify-center">
          <img
            src="https://raw.githubusercontent.com/pnxl/teyvat/master/assets/blog/images/quilt-setup/Screenshot%202022-06-17%20at%2007.24.58.png"
            alt="Minecraft launcher profiles"
          />
        </div>
        <p>a folder containing your Minecraft files will open.</p>
        <p>
          double-click the <span class="font-bold italic">mods</span> folder,
          and copy the mods you've extracted into the folder.
        </p>
        <p>once you're done, it should look a little something like this:</p>
        <img
          src="https://raw.githubusercontent.com/pnxl/teyvat/master/assets/blog/images/quilt-setup/Screenshot%202022-06-17%20at%2008.01.14.png"
          alt="mods folder"
        />
        <p class="text-sm">
          * NOTE: the contents may be different, as more mods get added into the
          server.
        </p>
      </div>
    </section>
    <section id="multimc" class="mb-16 space-y-4">
      <p class="text-lg font-light text-gray-400">MultiMC/UltimMC</p>
      <div class="space-y-2">
        <p>
          MultiMC makes installation of modloaders dead simple. before we start,
          make sure you have the following.
        </p>
        <br />
        <p class="font-light text-gray-400">pre-requisites</p>
        <ol class="ml-6 list-disc">
          <li>
            <a
              href="https://multimc.org/#Download"
              class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
              >MultiMC</a
            >
            or
            <a
              href="https://nightly.link/UltimMC/Launcher/workflows/main/main"
              class="font-medium text-blue-300 underline transition duration-150 hover:text-blue-200"
              >UltimMC</a
            >, of course
          </li>
        </ol>
        <br />
        <p class="font-light text-gray-400">Quilt installation</p>
        <p>
          first, create a new instance, name it whatever you want, with version
          1.19.
        </p>
        <p>on the right hand side, click on edit instance.</p>
        <p>then, click on the text that says "Install Quilt".</p>
        <p>click the latest available release, then click ok.</p>
        <p>you're done! don't close the window yet however.</p>
        <br />
        <p class="font-light text-gray-400">mod installation</p>
        <p>now, click on loader mods on the left side.</p>
        <p>
          extract the contents of the ZIP file you downloaded, preferrably onto
          a folder to keep your files from being messy.
        </p>
        <p>select all, and drag the mods you've extracted into said folder.</p>
        <p>once you're done, it should look a little something like this:</p>
        <img
          src="https://raw.githubusercontent.com/pnxl/teyvat/master/assets/blog/images/quilt-setup/Screenshot%202022-06-20%20at%2012.54.41.png"
          alt="mods folder"
        />
        <p class="text-sm">
          * NOTE: the contents may be different, as more mods get added into the
          server.
        </p>
      </div>
    </section>
    <section id="tlauncher" class="mb-16 space-y-4">
      <p class="text-lg font-light text-gray-400">TLauncher</p>
      <div class="space-y-2">
        <p>yeah no i don't think you can install quilt on tl lmao</p>
        <p>
          actually i think you can -- try following the minecraft launcher
          method
        </p>
        <p>but idk ¯\_(ツ)_/¯</p>
      </div>
    </section>
  </main>
</template>
