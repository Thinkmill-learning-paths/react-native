# React Native

## Foundation 5 - Create App

> View React Native's official docs - [React Native CLI Quickstart](https://reactnative.dev/docs/environment-setup)

### Create a new project - React Native

> Note, if this is your first time creating a React Native app on your machine, there are additional installation steps. See Official docs - ["Setting up the development environment"](https://reactnative.dev/docs/environment-setup).

1. Create a new app:

```
npx react-native init MyProject
```

Or create with TypeScript:

```
npx react-native init MyTSProject --template react-native-template-typescript
```

2. Navigate in to project, and to run in iOS simulator:

```
yarn ios
```

This will run both an iOS (backend) server and the JavaScript (frontend) server (Metro Bundler).

> ⚠️ If for any reason this throws a CLI exception, first read the exception and try to mitigate or for more verbose exception messages, run the app via Xcode.

Or to run the Android simulator:

```
yarn android
```

This runs both an Android (backend) server and the JavaScript (frontend) server (Metro Bundler).

> ⚠️ If for any reason this throws a CLI exception, open Android Studio and troubleshoot by running through Android Studio.

> ℹ️ `yarn start` on the other hand will run the JavaScript Metro Bundler server, and not a platform backend. Therefore it does not launch a simulator-based development environment.

3. To work, open the MyProject directory in your JavaScript code editor. Edit only the JavaScript files, not contents of ios/ or android/ directly, as many of these files contain generated code managed by editing via via Xcode or Android Studio (see Foundation 7 - Running a dev loop).

### Create a new project - Expo

1. Create a new Expo app:

```
npx expo init MyExpoApp
```

2. Launch the development environment, in iOS simulator:

```
cd MyExpoApp
yarn ios
```

or in Android simulator:

```
cd MyExpoApp
yarn android
```

This will launch a JavaScript development for the app in the platform's simulator.
