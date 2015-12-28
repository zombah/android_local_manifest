Local manifest to build CyanogenMod 12.1 UNOFFICIAL for [Nokia X2 aka Ara](http://4pda.ru/forum/index.php?showtopic=651024)

How to download:
-------------

Initialize repo:

    repo init -u git://github.com/CyanogenMod/android.git -b cm-12.1
    curl --create-dirs -L -o .repo/local_manifests/local_manifest.xml -O -L https://raw.githubusercontent.com/zombah/android_local_manifest_cm-nokia-x2/cm-12.1-test/local_manifest.xml
    repo sync


How to compile:
------------

    source ./build/envsetup.sh
    lunch cm_ara-userdebug
    make otapackage
