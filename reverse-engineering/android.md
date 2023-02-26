# Android

`apktool d android.apk` - extract apk file

`apktool b android.apk -o new.apk` - build apk file

`jadx-gui android.apk` - show apk files



## Dalvik opcodes

{% embed url="http://pallergabor.uw.hu/androidblog/dalvik_opcodes.html" %}

`keytool -genkey -v -keystore my-release-key.keystore -alias modified_apk -keyalg RSA -keysize 2048 -validity 10000`



`jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore my-release-key.keystore modified.apk modified_apk`
