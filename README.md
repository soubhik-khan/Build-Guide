# Build-Guide


to change version name/ date :
---------------------------------
nano vendor/cm/config/common.mk

to change ota link:
---------------------------------
https://github.com/CyanogenMod/android_packages_apps_CMUpdater


How to cherry-pick :
----------------------------------
git remote add upstream [repo link]

git fetch upstream [branch name]

git cherry-pick [sha of commit]

cd packages/apps/Profiles && git revert ea4e0f404b36afa8c37829dac0a8aea5b5a1a963 && cd ../../..


build steps:
-----------------------------------
make clean

repo sync

repo sync -c -f -j8 --force-sync --no-clone-bundle --no-tags

source build/envsetup.sh

breakfast tomato

make clean

brunch tomato

-------------------------------------------------


sftp://username@[ip address]/home/[username]

TO UPLOAD - go to the out folder
---------------------------------------
ftp uploads.androidfilehost.com

ftp basketbuild.com

put [file name.zip]

