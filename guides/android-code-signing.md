# Android code signing

To create a build or a release you need access to .keystore file to sign the code.

Keystore files should be located at "android/app/debug.keystore" and "android/app/release.keystore". You can commit them or optionally store them in a Password Manager and not check them in to git.

Password and key alias are currently stored at "signingConfigs" section of module build.gradle (android/app/build.gradle:149). The internal test one is "debug", the Play store release one is at "release". You can [optionally secure these to environment variables](https://stackoverflow.com/questions/41691000/how-to-store-android-keystore-passwords-securely).

## (Optional) How to regenerate a keystore file

You do not need to now, but if you wanted to regenerate the secure keys.

Generate a keystore file created from project root with this command:

    keytool -genkeypair -v -keystore android/app/debug.keystore -alias debug -keyalg RSA -keysize 2048 -validity 10000

## Build and distribute Android for internal test

### Authorisation (once)

You must have access to the debug.keystore file, it should be located at android/app/debug.keystore.

### Build

You can now build.

### Distribute

1. Bump the App version, open android/app/build.gradle and edit defaultConfig.versionName and/or defaultConfig.versionCode.

```
versionCode 21
versionName "1.0.3"
```

2. Generate an APK for distribution by file transfer (Build -> Generate Signed Bundle or APK).
   - 1. Choose "APK" (instead of Android App Bundle)
   - 2. The keystore file and passwords are found here: \_\_secure/android
   - 3. Choose "Release" build variant (this way you wont distribute a version with RN dev tools)
   - 4. Select both checkboxes for Signature Versions "V1 (Jar Signature)" and "V2 (Full APK Signature)"
3. A successfully generated build is found at:
   - android/app/release/app-release.apk, or
4. Transfer the file to stakeholders, and simply opening that file on an Android phone will install it.

## Distribute to the Google Play Store

### Authorisation (once)

You must have access to the release.keystore file, it should be located at android/app/debug.keystore.

You need to be added as a {company name} Android Developer.

1. {company name} will have a Google Developer Account, if not they can create one [here](https://play.google.com/apps/publish/signup/).

2. Ask to be added to the Account for the App as an Admin. Once this happens, you will receive an Email Invitation to the Publishing area -> [more on this](https://support.google.com/googleplay/androiddeveloper/answer/2528691?hl=en)

3. Verify you are added by signing in to [Google Play Publishing Console](https://play.google.com/apps/publish)

// todo

Docs -> https://developer.android.com/studio/publish/app-signing
Docs -> https://developer.android.com/studio/publish/app-signing#sign_release

### Publish

Publish to the Google Play Store.

// todo

## Links

- React Native's [Official Guide](https://reactnative.dev/docs/signed-apk-android)

- What's the difference between [Signature Versions](https://stackoverflow.com/questions/42648499/difference-between-signature-versions-v1-jar-signature-and-v2-full-apk-sign)?

- [Generating a new keystore file](Documentation: https://reactnative.dev/docs/signed-apk-android)

- Android's [Official Publishing Release Docs](https://developer.android.com/studio/publish#publishing-release_)
  https://reactnative.dev/docs/signed-apk-android#generating-an-upload-key
