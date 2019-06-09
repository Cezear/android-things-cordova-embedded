# Android Things: Cordova Embedded
This repository is a fork of [Android-Cordova-Embedded](https://github.com/Cezear/android-cordova-embedded) that has been configured to run on [Android Things](https://developer.android.com/things) devices.

## What has changed?
The most surprising new addition is the Android Things dependency, which has been added to `build.gradle (Module: app)` and configured in the `AndroidManifest.xml` to not be required so that the application can be quickly deployed on emulators.

Also within the `build.gradle (Module: app)` configuration `minSdkVersion` has been increased to 25 to meet Android Things compliances; the application will attempt to use version 28 for compiling and 29 for build tools.

## Android Things platform differences
Android Things was designed to be as cross-compatible as possible with the original Android OS; so this means that most plugins offered with Cordova will work on Android Things. This [plugin status](https://github.com/intel-iot-devkit/android-things-cordova/blob/master/plugins_status.md) page provided by Intel IoT provides an (I assume) up-to-date record on the plugins that do and do not work on the platform.
