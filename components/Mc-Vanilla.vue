<template>
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
      first, you should at least start Minecraft 1.19 once, to make sure that
      you've downloaded all needed files for Quilt to patch.
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
      now, open the Minecraft launcher and you should see a new profile named
      <span class="font-semibold italic">quilt-loader-1.19</span>.
    </p>
    <p>
      if that's the case, congratulations! you've sucessfully installed Quilt
      onto Minecraft.
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
      extract the contents of the ZIP file you downloaded, preferrably onto a
      folder to keep your files from being messy.
    </p>
    <p>
      now, click on the Installations tab on the Minecraft launcher, hover over
      your Quilt profile and click on the folder icon.
    </p>
    <div class="flex flex-row justify-center">
      <img
        src="https://raw.githubusercontent.com/pnxl/teyvat/master/assets/blog/images/quilt-setup/Screenshot%202022-06-17%20at%2007.24.58.png"
        alt="Minecraft launcher profiles"
      />
    </div>
    <p>a folder containing your Minecraft files will open.</p>
    <p>
      double-click the <span class="font-bold italic">mods</span> folder, and
      copy the mods you've extracted into the folder.
    </p>
  </div>
</template>
