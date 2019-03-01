# Cordova-Hello-World
Cordova Hello World

[More on cordova.apache.org](https://cordova.apache.org/docs/en/latest/guide/overview/index.html)

For DB look at [Lokijs](http://lokijs.org) & [Taffy](http://taffydb.com/).
## Run
```
cordova serve
```

## Add Platforms

```
cordova platform add windows
cordova platform add osx
cordova platform add ios
cordova platform add android
```

## Build for Platform

```
cordova build browser
cordova build windows
cordova build osx
cordova build ios
cordova build android
```

## Troubleshoot

### Linux

> No installed build tools found. Install the Android build tools version 19.1.0 or higher.

```
sudo add-apt-repository ppa:maarten-fonville/android-build-tools
sudo apt-get update
sudo apt install android-sdk-build-tools
```

> Failed to apply plugin [id 'com.android.library']
> Minimum supported Gradle version is 4.10.1. Current version is 4.1. If using the gradle wrapper, try editing the distributionUrl in /home/mike/Documents/Projects/Cordova/Cordova-Hello-World/gradle/wrapper/gradle-wrapper.properties to gradle-4.10.1-all.zip

```
sudo apt install apt-transport-https dirmngr wget software-properties-common
sudo add-apt-repository ppa:cwchien/gradle
sudo apt update
sudo apt install gradle
gradle -v
```
