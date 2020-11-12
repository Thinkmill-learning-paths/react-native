# Setting up iOS

1. Set up your environment for the React Native CLI (not Expo) as described in the [official docs](https://reactnative.dev/docs/next/environment-setup).

2. Be sure to sign in to Xcode with your Apple ID, Xcode -> Preferences -> Accounts

3. Open `./ios/worrytime.xcworkspace` in Xcode

4. Install Pods (Xcode dependencies)

   i. If you ever need to bump the version of the Cocoapods you have installed,

   Depending on how you installed Cocoapods:

   `sudo gem install cocoapods -v 1.9.1`

   or

   `brew install cocoapods@1.9.1`

```
cd ios
pod install
```

## Links

Developer docs http://developer.apple.com/

Manage your Apple ID at https://appleid.apple.com/

Manager your iOS App at https://appstoreconnect.apple.com/
