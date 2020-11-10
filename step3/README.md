# React Native

## Step 3 - Data management

In a React Native app there are a range of data storage approaches that might be appropriate for your use case.

If your app needs only session based data, then you can simply use a React Context to store your data at runtime.

However, if you would like to store data across sessions but local to the device, `AsyncStorage` is a great option. You can think of `<AsyncStorage>` like `window.localStorage` in Web. This data however, can be deleted in phone settings.

If your needs are formal storage, or multi device storage, you would look to persisting data to a web service backend.

### Task 1
