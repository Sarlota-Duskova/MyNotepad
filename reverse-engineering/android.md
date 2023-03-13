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

Run command line:

`adb shell`

`run-as com.insecureshop`

`ls -al`

## APK file structure

![](../.gitbook/assets/image.png)

**Manifest file:** An additional Android manifest file, describing the name, version, access rights, referenced library files for the application. This file may be in Android binary XML that can be converted into human-readable plaintext XML with tools such as AXMLPrinter2, apktool, or Androguard.

**Signatures (META-INF):** It contains the Certificates and the signatures.

**Assets:** A directory containing applications assets, which can be retrieved by AssetManager.

**Compiled resources(resources.arsc):** A file containing precompiled resources, such as binary XML for example.

**Native Libraries(lib):** The directory containing the compiled code that is platform dependent; the directory is split into more directories within it:

* `armeabi-v7a`: compiled code for all ARMv7 and above based processors only
* `arm64-v8a`: compiled code for all ARMv8 arm64 and above based processors only
* `x86`: compiled code for x86 processors only
* `x86_64`: compiled code for x86 64 processors only

**Dalvik bytecode(class.dex):** The classes compiled in the dex file format understandable by the Dalvik virtual machine and by the Android Runtime.

**Resources(res):** the directory containing resources not compiled into resources.arsc



## What to look for

#### Exploring the Android Manifest

* **debuggable** - the app being in debug mode, meaning it’s possible to attach a debugger to the application’s process and execute arbitrary code.
* **allowBackup** - defines whether application data can be backed up and restored by a user who has enabled USB debugging. This means that hackers connecting to a device via adb can easily obtain any application data that is stored on the device, including personal data on private storage.

#### Searching for Hardcoded values

* Looking for hardcoded **secret** keys

#### Analyzing WebViews in an App

* setWebContentsDebuggingEnabled(true) - allows inspections of WebView content from a remote browser, so it must always be set to false.
* clearCache(true) - clears the WebView caches from the client device. This can mitigate issues relating to sensitive data stored on the local file system.
* EnableSafeBrowsing - displays warnings when a compromised or known phishing website is loaded in the WebView.





