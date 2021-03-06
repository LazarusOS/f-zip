# F-zip: Universal recovery flashable zip generator for Linux & android
## (c) sunilpaulmathew @ xda-developers.com

## What is F-zip about?
"F-zip is a universal shell script designed to make recovery flashable zip files with a few simple steps“

## For those it is helpful?
Anyone (devs/newbies) who has something (boot.img/apps/libs/bootanimation/framework) to flash and do not want to do all the work to make a recovery zip manually

## Where it works?
It will works on any Linux and Linux based operating systems including android. The Linux system might be native or with in a virtual box or even the bash inside Windows 10.

# How-to-use F-zip

## 1. clone or download f-zip repo into your Linux PC or Android device.
## 2. copy "boot.img", if any, into the root folder. Caution: Don’t forget to modify “fzip.sh” (line# 30), if your device is anything other than Samsung Galaxy S5 (kltexxx).
## 3. copy the app folder(s) in to "/system/priv-app/" or/and "system/app/". You may also copy the “.apk” file(s) directly to “/system/app/” or/and “/system/priv-app/” (without folder) if your app/ROM supports to do so.
## 4. copy library (typically “.so”) file(s), if any, into “/system/lib/”
## 5. copy modules (typically “.ko”) file(s), if any, into “/system/lib/modules/”
## 6. copy framework (typically “.jar”) file(s), if any, into “/system/framework/”
## 7. copy "framework-res.apk", if any, into “/system/framework/”
## 8. copy "bootanimation.zip" (only for aosp ROMs) file, if any, into “/system/media/”
## 9. modify fzip.sh accordingly (please see instructions below)
## 10. open terminal and cd to the root folder of f-zip
## 11. run ". fzip.sh" (in Linux) or “sh fzip.sh” (in android).
## 12. The recovery flashable zip file will be generated in the root folder.

## [How-to-modify shell script?](https://github.com/SmartPack/f-zip/blob/master/How-to-modify.md)
