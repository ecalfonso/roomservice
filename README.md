SaberMod CM12.x for jflte devices

Start your build environment with this tutorial here: http://wiki.cyanogenmod.org/w/Build_for_jfltexx

Required repos:
Placing the *.xml files in this repo will allow you to build SaberMod Optimized CyanogenMod for the Galaxy S4 Snapdragon Variants

  Bloat.xml - Removes some unecesarry repos from being synced. Reduces repo sync time and space required for the source
  Common.xml - Commonly shared repos between CM supported devices
  jflte.xml - Repos for unified Samsung Galaxy S4 devices
  flo.xml - Repos for the Google Nexus 7 (2013) - NOT REQUIRED FOR BUILDING FOR JF - Buildable, but not bootable

Place these files in your ~/android/system/.repo/local_manifests/ folder (if you followed the linked tutorial)

SaberMod Toolchains:
ROM toolchains can be found here: http://sabermod.com/Toolchains%20%28DEV%20ONLY%29/arm/arm-linux-androideabi/
Kernel toolchains can be found here: http://sabermod.com/Toolchains%20%28DEV%20ONLY%29/arm/arm-eabi/

Unzip toolchains into your ~/android/system/prebuilts/gcc/linux-x86/arm/ folder

Where to declare which toolchina to use: https://github.com/xsynergy510x/android_vendor_sabermod/blob/cm-12.1/device/sm_jflte.mk#L27-28

From here you should be able to repo sync the source and build for SaberModCM12.x for jflte!
