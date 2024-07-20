Welcome to CandyRoms
===================


Begin tasting the sweetness
---------------

To get started with CandyROMs based on Android 14, you should be familiar with
[Git and Repo](https://source.android.com/source/using-repo.html) and the basics of internal Android functionality.

Please set up your build environment by following the [AOSP guide](https://source.android.com/setup/build/initializing).

You might want to take a look at @akhilnarang's scripts [here](https://github.com/akhilnarang/scripts).

To initialize your local repository using the Candy c14 trees, use this command:


    repo init -u https://github.com/CandyRoms/manifest.git -b c14


Then sync up with this command:

    repo sync

Additional flags which you can append to speedup the sync process are:

    repo sync --force-sync -c --no-tags --no-clone-bundle --optimized-fetch --prune -j$(nproc)

To make Candy:

    source build/envsetup.sh
    lunch candy_device-userdebug
    make bacon


Official Device Support
-----------------------

We only support the devices we own.

If you are interested in becoming an "official" Device Maintainer or a part of the team, you are welcome, but we have some basic expectations of a DM, but nothing too crazy.  We want to avoid "one hit wonders" that come and go just as fast. So be prepared to show us at least a few months of your source code activities, with proper authorship. You should also be able to use Gerrit code review to push and pick/pull changes.

If you are a device maintainer, want to build/support your device on CandyRoms, and can meet our DM requirements please contact us to be considered.

We mostly need to see some history of your activity, how you use Github (and Gerrit), and maintain authorship.  User interaction is considered too, as well as bug fixing and timeframes to do so, so a release channel where you post your work should be present.
