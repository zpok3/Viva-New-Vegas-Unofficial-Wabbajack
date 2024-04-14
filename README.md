<img src= "https://github.com/zpok3/Viva-New-Vegas-Unofficial-Wabbajack/blob/main/background.webp" target="_blank"></a>

# Unofficial Viva New Vegas Wabbajack
---

<p align="center">
 <a href="https://vivanewvegas.moddinglinked.com/">Home Page</a> ·
  <a href="https://vivanewvegas.moddinglinked.com/wabbajack.html">Official VNV WJ Readme</a>

---

# Introduction

Please read [here](https://vivanewvegas.moddinglinked.com/intro.html) for an overview to the modlist along with its requirements and recommended specs.

# Setup

Please read [here](https://vivanewvegas.moddinglinked.com/setup.html) for instructions on how to properly do a clean installation of the game. Next, follow these steps to install the Wabbajack:

1. Create a folder outside of any default Windows folders (I recommend `C:\Modding\Viva New Vegas`) - this is where the list will be installed to.

2. In the Wabbajack app select `Install From Disk`

3. In the `Target Modlist` box, navigate to the location you downloaded `Viva.New.Vegas.wabbajack` to.

4. In the `Mod List Installation Location` box, select the folder you created in step one. The resources download location should fill automatically - you can change it to another drive if you're short on space.

5. Click the start button and wait for Wabbajack to finish.

# Post Installation Steps

**FNV4GB Patcher:**
1. Under the `Post Installation` separator in MO2, right click on the mod `FNV 4GB Patcher` and select `Open in Explorer`

2. Copy `FNVpatch.exe` to your game's `root` folder.

3. Double click on the exe to run it.

4. A command prompt window will open and should say `FalloutNV.exe patched!`

5. Close the command prompt and a file named `FalloutNV_backup.exe` should appear in the game's `Root` folder.

**NVTF:** If you are planning on adding texture mods, please enable `Texture Modding Preset` under the `Utilities` separator.

**Starting the MO2:** 
1. After running `ModOrganizer.exe` from the modlist installation directory, you will get an error regarding MO2 being unable to open instance 'Portable', select OK and select `New Vegas` from the list of games.

2. Select the version of the game (either Steam/GOG). You will likely get an error about how profile Default was not found and MO2 is using profile Viva New Vegas instead, select OK and continue.

3. Select `Do Nothing` when asked about Nexus categories.

4. You can change the theme in MO2's settings if you don't want to be flashbanged everytime you open MO2 - I recommend 1809 Dark Mode or vs15 Dark. Select 
<img src= "https://raw.githubusercontent.com/ModdingLinked/Viva-New-Vegas/master/img/mo2%20settings.webp" target="_blank"></a>
and go to the Themes tab if you'd like to do this.

## Optional Steps

**FPS Limiter:** Please follow the **Recommended Limiters** section of the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html#RecommendedLimiters) to massively reduce your latency (this is highly recommended because the Wabbajack only comes with VSync as default, which is not meant to be used as a limiter but we cannot provide a pre-configured one).

**DXVK:** Please follow the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html) for information on which DXVK version you should enable under the `Post Installation` separator. **(This is not optional for AMD users! The game will most likely crash if you don't follow this step.)** 

**BSA Decompressor:** The BSA Decompressor will give you slightly better performance and faster loading times at a small disk space cost.

1. Under the `Post Installation` separator in MO2, right click on the mod `FNV BSA Decompressor` and select `Open in Explorer`

2. Run `FNV BSA Decompressor.exe`

3. The Fallout: New Vegas and Decompressed Archives paths should be filled by default (root folder and data folder respectively). If they aren't, close the program and re-run your game launcher to generate the required registry key

4. Click Decompress, wait for the process the finish, then exit the program once finished

**NVHR:** Under the `Post Installation` separator in MO2, copy the contents of the mod `New Vegas Heap Replacer` to your game's `root` folder.
