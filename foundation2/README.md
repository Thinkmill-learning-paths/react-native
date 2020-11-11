# React Native

## Foundation 2 - Key differences to Web

- Exceptions
- Offline-ness

- Data persistence
- Styling

- native apis, fetch, date

React Native has a different document object model, and so has its own native components. For example, in React Native, there is no such thing as a `<div>` element, instead you would use `<View>`. Similarly, there is no `<a>`, rather we can use `<Button>` or other Touchable components. Similarly, there is no '<p>', rather we can use '<Text>".

Under the hood, React Native's Components internally map to iOS or Android native elements.

In a React Native app there are a range of data storage approaches that might be appropriate for your use case.

If your app needs only session based data, then you can simply use a React Context to store your data at runtime.

However, if you would like to store data across sessions but local to the device, `AsyncStorage` is a great option. You can think of `<AsyncStorage>` like `window.localStorage` in Web. This data however, can be deleted in phone settings.

If your needs are formal storage, or multi device storage, you would look to persisting data to a web service backend.

### Task 1

DO USE ASYNC STORAGE WHEN... DON'T USE ASYNC STORAGE FOR...
Persisting non-sensitive data across app runs Token storage
Persisting Redux state Secrets
Persisting GraphQL state
Storing global app-wide variables

https://github.com/oblador/react-native-keychain
