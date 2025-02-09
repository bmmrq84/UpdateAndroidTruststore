# UpdateAndroidTruststore
Magisk module to update android truststore

Systemlessly replace system Root CA certificates with [latest from AOSP source](https://android.googlesource.com/platform/system/ca-certificates/+archive/refs/heads/main/files.tar.gz)

Use this if you have an out of support Android device still supported by [Magisk](https://github.com/topjohnwu/Magisk)

Symptoms cured by this module (all are same symptom under the hood, SSL/TLS errors):
- Some websites cannot be loaded
- Some Apps could not use internet

ATTENTION: Will only work if android system truststore is located in /system/etc/security/cacerts

Reference: [XDA discussion](https://xdaforums.com/t/modern-browser-for-android-kitkat-4-4-4.4634649)

This is a very simple module without code or scripts. It just uses magisk overlay capabilities.

Tested successfully using a Shield Tablet K1 Stock 5.4 (Android 7.0).

Enjoy!
