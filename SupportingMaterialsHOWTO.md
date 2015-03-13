# Collecting Supporting Materials1 #
Prior to posting an issue, please collect supporting materials so that the developers can attempt to reproduce the problem. Some examples of supporting materials include logcat and dmesg output, and in the case of media (audio/video) errors, a link to the file in question. Please follow the steps below to collect logcat and dmesg output using adb or the pre-installed Terminal Emulator application.

## Collecting logs using ADB ##
ADB is the fastest way to collect logs. In order to use ADB, you need to have the Android SDK installed and, if using Windows, the SDK drivers installed. Please use the following commands to collect logcat and dmesg from the command line:

```
adb logcat -d > logcat-output.txt
adb shell dmesg > dmesg-output.txt
```

## Collecting logs using Terminal Emulator ##
Start Terminal Emulator
Type the following commands:

```
logcat -d > /sdcard/logcat-output.txt
dmesg > /sdcard/dmesg-output.txt
```

Enable USB Storage mode and copy the files off of your phone.