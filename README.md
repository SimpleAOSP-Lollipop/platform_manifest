SimpleAOSP Github
===================

Setting up Build Environment
---------------------------
- Please see the [Android source page](http://source.android.com/source/index.html) for building instructions

Initializing the Source
-----------------------
(Assuming you have a valid build environment setup)
- mkdir simpleaosp
- cd ~/simpleaosp
- repo init -u https://github.com/SimpleAOSP-Lollipop/platform_manifest.git -b L

Sync the Source
---------------
- repo sync -jx -f (x being however many cpu jobs)

Getting Ready to Build
----------------------
- . build/envsetup.sh

Choose Supported Device to Build
--------------------------------
- lunch simpleaosp_flo-user 
- lunch simpleaosp_hammerhead-user
- lunch simpleaosp_mako-user
- lunch simpleaosp_shamu-user

Now Build it
------------
- mka otapackage

For Quick Dirty Rebuilds
------------------------
- cd ~/simpleaosp
- repo sync -jx -f (x being however many cpu jobs)
- lunch and pick the right device (refer to above for choosing right device to build)
- mka dirty
- mka otapackage

Credits
-------
- Google for AOSP
- Rascarlo and RastaPop
- Altaf-Mahdi and Euphoria-OS
- DariosF and Purity ROM
- Paranoid Android (AOSPA)
- AOSPAL
- CyanogenMod
- Dirty Unicorns
- LiquidSmooth
- AOKP
- SlimROMS
- Project D.I.S.C.O. Team
- PartimusPrime for bootanimations
- OmniROM
- Lichti1901 and Terminus
- Sykopompos
- Team Horizon and XenonHD
- Chet and OptiPop
- VanirAOSP
- Others we may have missed
