# Installing native plugins

Both platforms now support [autolinking](https://github.com/react-native-community/cli/blob/master/docs/autolinking.md).

You still need to thoroughly read installation steps for each plugin, but you should not need to run a `react-native link` or copy and past the output of that process, you can test what that would like like with:

    yarn react-native link --platforms android react-native-config
