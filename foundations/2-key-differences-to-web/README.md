# React Native

## Foundation 2 - Key differences to Web

### Document object model

React Native has a different document object model to the browser.

There are no HTML elements in React Native, instead we are provided Core Components. For example, `<View>` in place of `<div>`, `<Text>` in place of `<p>`, and others.

> React Native docs - [Core Components and Native Components](https://reactnative.dev/docs/intro-react-native-components)

### JavaScript engine

React Native has a different JavaScript engine to the browser, rather than V8 it uses JavaScriptCore. It includes a subset of language features.

There is an absence of `window` or `document` and there are some features missing for example, there is no `localStorage` or `sessionStorage`. Storage alternatives are available as plugins, namely [AsyncStorage](https://github.com/react-native-community/react-native-async-storage) and [React Native Keychain](https://github.com/oblador/react-native-keychain).

Some modern language features however are polyfilled including `fetch`.

> React Native docs - [JavaScript Environment](https://reactnative.dev/docs/javascript-environment)

### Styling

React Native has a subset of styles available to use, and its own syntax for creating style sheets.

> React Native docs - [Style](https://reactnative.dev/docs/style)

A most notable difference to web is layout, React Native uses flexbox entirely to lay out elements, as there is `display` property.

> Handy visual tool for creating React Native flexbox code - [Yoga](https://yogalayout.com/playground/)

### Platforms

React Native can build apps for various Apple or Google platforms, including phone apps, smart devices like iWatch, desktop apps, and tv apps.

React Native in combination with [React Native Web](https://github.com/necolas/react-native-web) can even build web apps. If you want to build a universal app, you might consider using Expo.

## Mobile environment

When building mobiles apps, thinking about how the lifecycle of your app will help you account for more of the ways it will be used.

For example:

- [`AppState`](https://reactnative.dev/docs/appstate) tells us whether the app is closed, in the foreground or the background - will this impact your app flow?
- Mobile devices are likely to experience offline usage - will your app work offline?
- Mobile app's runtime does not recover from exceptions - how will you defend your app from crashing?
