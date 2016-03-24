Example OS-Agnostic Summon App
==============================

Mobile phone user interface example. Works with
[Summon](https://github.com/lab11/summon) on Android and iOS.
This app can be pointed to from an Eddystone packet to serve the user
interface. The link is [goo.gl/hWTo8W](goo.gl/hWTo8W)



To rebuild everything:

    ./init_cordova.sh

To build and run on attached phone:

First temporarily change loading of `cordova.js` to `cordova_test.js` in index.html, then
```
    cd _build/
    cordova run android
```

To debug an attached android phone:
```
    adb logcat chromium:D *:S
```
