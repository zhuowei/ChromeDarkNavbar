An Android OMS theme for tinting the status bar of Chrome 64 on Android 8.1.

# Building and Installing

This isn't a Substratum theme: Substratum themes builds the final theme on device after applying customizations.

Because I don't have Substratum, I just directly built the OMS overlay APK.

- Place a copy of Chrome as chrome.apk in this directory
- gradlew assembleDebug
- adb install app/build/outputs/app-debug.apk
- adb shell cmd overlay enable net.zhuoweizhang.chromedarknavbar

# License

Apache 2.0.

# Additional notes

[The commit that added the light statusbar](https://chromium.googlesource.com/chromium/src/+/bd6f02339cb7c5bd405e0b15adcaf468ca8aa934)

[The tutorial I followed to make an OMS theme](https://code.tutsplus.com/tutorials/quick-tip-theme-android-with-the-runtime-resource-overlay-framework--cms-29708)
