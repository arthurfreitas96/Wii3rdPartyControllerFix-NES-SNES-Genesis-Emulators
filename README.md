# WiiClassicControllerPro-OffBrandFix
I bought an off-brand Wii Classic Controller Pro for 9 dollars and it was just plug and play for Wii, GC, and Virtual Console games. Moreover, I had no problems with it while playing emulated N64, either. However, while testing my controller in NES, SNES and Genesis/Mega Drive emulators, I experienced an extremely laggy output from it. I found a youtuber reviewing a controller (not the Pro though) and facing the same problems, here: https://www.youtube.com/watch?v=P9b4ZtHvlLs.
This issue was discussed in the following links:

snes9xgx (SNES emulator) dicussion:
https://github.com/dborth/snes9xgx/issues/947

genplusgx (Genesis emulator) discussion:
https://github.com/ekeeke/Genesis-Plus-GX/issues/334

As a result of the discussions, I managed to compile some builds of the following three emulators: fceugx, snes9xgx and genplusgx. These builds implement the changes applied to the source code in order to allow support to my off-brand controller, fixing the laggy output issue.

Usage: place the emulator's .dol file in a folder (name the folder after the emulator, any name will do) inside your apps folder and rename the .dol to boot.dol.

Compilation instructions:

To compile the three emulators, I recommend using devkitPRO-pacman, latest version. Install the following packages on it: ppc-bzip2 ppc-freetype ppc-libjpeg-turbo ppc-libogg ppc-libpng ppc-libvorbisidec ppc-mpg123 ppc-mxml ppc-pkg-config ppc-zlib. Replace the standard libogc by the modded one provided in this directory. To compile genplusgx, you will need to replace the standard devkitPPC by the devkitPPC r29-1, provided here: https://wii.leseratte10.de/devkitPro/devkitPPC/r29-1%20(2017)/.
