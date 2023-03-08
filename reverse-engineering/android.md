# Android

`apktool d android.apk` - extract apk file

`apktool b android.apk -o new.apk` - build apk file

`jadx-gui android.apk` - show apk files

Extract backup file:

```bash
( printf "\x1f\x8b\x08\x00\x00\x00\x00\x00" ; tail -c +25 backup.ab ) |  tar xfvz -
```



## Dalvik opcodes

{% embed url="http://pallergabor.uw.hu/androidblog/dalvik_opcodes.html" %}

Create key to validation of application:

`keytool -genkey -v -keystore my-release-key.keystore -alias modified_apk -keyalg RSA -keysize 2048 -validity 10000`

Application can be signed by:

* jarsigner
* zipalign

Validate an application with created key:

`jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore my-release-key.keystore modified.apk modified_apk`

Is a android optimalization:

`zipalign -v 4 application.apk signed.apk`

signed.apk - is output apk file

4 - provides 32-bit alignment



## Tools

* ADB
* ApkTool
* uber-apk-signer
* ApkStudio
* Idea
* IdeaSmali

### Profiling tools (root required)

* Frida
* Introspy
* Xposed

### Automated tools

* Mobile Security Framework (MobSF)
* Quick Android Review Kit (QARK)
* Drozer

### Finding and exploiting URL handlers

**Command:**

`find . -name AppDelegate.swift`

**Output:**

For Swift:

./DVIA-v2/AppDelegate.swift

or for Objective C

./DVIA-v2/AppDelegate.m

### Android Studio

Use bar Tools -> SDK Manager then copy Android SDK Location, open terminal and direct to that path then add:&#x20;

`adb install oauth.apk`

then in command line I can start attack:

`adb shell am start -d "oauth://final/?uri=https://sarlota-duskova.github.io/CTF/oauthbreaker/"`









