# React Native

## Foundation 1 - Key differences to React

React Native apps require React, and React's full API is available.

In addition to React, the React Native library provides components and API's for building in the native environment. Whereas in web, the browser provides components and API's.

For example, a React app:

```
import React from 'react';

const App = () => (
  <div>
    <p>Hello world</p>
  </div>
)
```

A React Native app:

```
import React from 'react';
import { View, Text } from 'react-native';

const App = () => (
  <View>
    <Text>Hello world</p>
  </View>
)
```
