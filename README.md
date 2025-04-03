<img src= "https://github.com/zpok3/Viva-New-Vegas-Unofficial-Wabbajack/blob/main/background.webp" target="_blank"></a>

# Unofficial Viva New Vegas Wabbajack
---

<p align="center">
· <a href="https://vivanewvegas.moddinglinked.com/">Home Page</a> ·
  <a href="https://vivanewvegas.moddinglinked.com/wabbajack.html">Official VNV WJ Readme</a> ·

---

# Introduction

**Update: The official Wabbajack is back so this will no longer be supported unless Vish deletes it again**

Please read everything carefully (both this readme and any pages to Viva New Vegas that are linked), you can **NOT** skip steps and expect your game to function as it should! Please read [here](https://vivanewvegas.moddinglinked.com/intro.html) for an overview of the modlist along with its requirements and recommended specs.

# Requirements

* The requirements listed in [Viva New Vegas](https://vivanewvegas.moddinglinked.com/intro.html#requirements)

* The latest release of [Wabbajack](https://www.wabbajack.org/)
* The latest wabbajack file for this list downloaded from the [Releases](https://github.com/zpok3/Viva-New-Vegas-Unofficial-Wabbajack/releases) page.

# Setup

> [!important]
> ## Clean Installation
> Please read the [Setup](https://vivanewvegas.moddinglinked.com/setup.html) section of Viva New Vegas for instructions on how to properly do a clean installation of the game, along with generating fresh INI files. The game must be installed out of any default Windows folders, such as `Program Files (x86)` or your `Desktop`.

## Installation

1. Create a folder for Wabbajack outside of any default Windows folders.

Example: `C:\Modding\Wabbajack`

2. Place the downloaded Wabbajack.exe in this folder and run it.
3. Select `Install from Disk` in the Wabbajack app. You will have to manually select where you downloaded the .wabbajack file in the `Target Modlist` box.
4. In **Installation Location**, select a folder that is not:
  * The Steam folder,
  * Any default Windows folders,
  * The Game folder,
  * The folder where you put Wabbajack.exe.

Example: `C:\Modding\Viva New Vegas`

5. **Begin** the installation.
6. Accept the Nexus Mods API request.
7. If you are not a Premium user you will need to manually click download for each mod.
8. Once complete Wabbajack, will show a green **Installation Complete** screen.
  * If you see a red **Installation Failed** screen, try log-in again through the Wabbajack settings, then reinstall the list to the same folder.

# Post Installation Steps

The latest version of the list has been reformatted to have the same post install procedure as the official [VNV Wabbajack](https://vivanewvegas.moddinglinked.com/wabbajack.html#PostInstallSteps). These steps are for versions **25.4.24 Update 1** and earlier.

## Exclusions
1. Open Windows Security.
2. Open **Virus and Threat Protection**.
3. Click **Manage Settings** under **Virus and threat Protection settings**.
4. Scroll down and click **Add or remove exclusions** under **Exclusions**.
5. Add a **Folder** exclusion and point it to the **Installation Location** folder.
  * If you are using a third-party antivirus, you will need to find the exclusions menu and add one to the same folder.

## 4GB Patcher
1. Under the `Post Installation` separator in MO2, right click on the mod `FNV 4GB Patcher` and select `Open in Explorer`

2. Copy `FNVpatch.exe` to your game's **Root** folder (the folder where the game is installed).

3. Double click on the exe to run it.

4. A command prompt window will open and should say `FalloutNV.exe patched!`

5. Close the command prompt and a file named `FalloutNV_backup.exe` should appear in the game's `Root` folder.

## NVTF
If you are planning on adding texture mods, please enable `Texture Modding Preset` under the `Utilities` separator.

## Configuring Game Settings
1. Open the game launcher using the `Fallout Launcher` option in MO2.
2. Inside the launcher click `Options` and do the following:
    1. Select `Ultra` preset.
* If you have a very weak PC, you can select the `Medium` preset instead.

  2. Set `Resolution` to your monitor's native resolution.
* If you can't find the right resolution in the launcher's list, do the following:
    
    1. Close the launcher.
    2. Click the <img src= "https://raw.githubusercontent.com/zpok3/Waters-of-Life/main/images/tools%20menu.webp" target="_blank"></a> button and select `INI Editor`.
    3. Select the `FalloutPrefs.ini` tab.
    4. Change the following settings in the `[Display]` section:
    * `iSize W` = your screen width
    * `iSize H` = your screen height
3. Close the launcher.

Additionally if you use an ultrawide monitor, follow these additional steps:

Ingame, go to `Settings -> Tweaks` and search for `Ultrawide`. Enable the Ultrawide Support tweak by clicking it in the panel on the lefthand side, then exit and restart the game so it takes effect.

## BSA Decompressor 
Decompresses the vanilla BSA files to reduce loading times and stuttering. Can also fix certain sound effects not playing.

1. Under the `Post Installation` separator in MO2, right click on the mod `FNV BSA Decompressor` and select `Open in Explorer`

2. Run `FNV BSA Decompressor.exe`

3. The Fallout: New Vegas and Decompressed Archives paths should be filled by default (root folder and data folder respectively). If they aren't, close the program and re-run your game launcher to generate the required registry key

4. Click Decompress, wait for the process the finish, then exit the program once finished

## Performance Guide

**Cap your FPS:** Please follow the **Recommended Limiters** section of the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html#RecommendedLimiters) to massively reduce your latency (this is highly recommended because the Wabbajack only comes with VSync as default, which is not meant to be used as a limiter but I cannot provide a pre-configured one).

- **DXVK with DXGI**: Highly recommended if you want improved input latency and VRR support.  Version 2.0 of DXVK requires a GPU that supports Vulkan 1.3 - if you have an AMD Radeon RX 400 series or newer (except RX 455 OEM), NVIDIA GeForce 900 series or newer, or Intel HD 510/530 or newer you should be able to use DXVK 2.0 (source: [TechPowerUp GPU Database](https://www.techpowerup.com/gpu-specs/)).
  - If you use an AMD GPU, all you have to do is enable the mod `DXVK` under the `Post Installation` separator in MO2. If you use a Nvidia GPU you'll also need to follow steps 2-6 under [**Enabling Flip Model (DXVK with DXGI)**](https://performance.moddinglinked.com/falloutnv.html#DXVK).
  - If you have issues with the latest version or your GPU doesn't support Vulkan 1.3 you can try the 1.10.3 version. If you are having issues on an Intel iGPU you can try the 1.10.1 version.
For more information on DXVK, VRR, HDR, and Alt-Tabbing, please refer to the [Performance Guide](https://performance.moddinglinked.com/falloutnv.html). 

# Updating the List

1. Download the latest version of the Wabbajack list from the [Releases](https://github.com/zpok3/Viva-New-Vegas-Unofficial-Wabbajack/releases) page.

2. In the Wabbajack app, select `Install From Disk`

3. In the `Target Modlist` box, navigate to the location you downloaded `Viva.New.Vegas.wabbajack` to.

4. Tick the `Overwrite Installation` box underneath the start button.

5. Make sure the contents of the `Mod List Installation Location` box match where you originally installed the modlist before clicking the start button.
