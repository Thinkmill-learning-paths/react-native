## Error: port already in use

Error:
`error listen EADDRINUSE: address already in use :::8081. Run CLI with --verbose flag for more details.`

Find the id for the process that is listening on port 8081:

```
lsof -i :8081
```

Then run the following to terminate the process:

```
kill -9 <PID>
```

## Reset cache

`yarn clean` (react-native-clean-project)

or

- Remove the iOS build - `rm -rf ios/build`
- Remove node modules - `rm -rf node_modules`
- Clear yarn's cache - `yarn cache clean`
- Delete all Watchman - `watchman watch-del-all`
- Remove react cache - `rm -rf $TMPDIR/react-*`
- Remove haste cache - `rm -rf $TMPDIR/haste-map-*`
- Remove metro cache (sort of like RN webpack) - `rm -rf $TMPDIR/metro-cache-*`
- Delete pods - `rm -rf ios/Pods`
- If all else fails `yarn start --reset-cache`

## Reset Android Studio's cache

You might need to do this if things go horribly wrong and you cant understand why Android Studio is throwing errors.

1. close the project (File -> Close Project)

2. close Android Studio IDE

3. delete the .idea directory (rm -rf android/.idea)

4. delete all .iml files (there are 2 inside ./android)

5. open Android Studio IDE and import the project

6. Invalidate Android Studio caches (File -> Invalidate Caches / Restart)

7. Reopen Android Studio, wait for operations to complete, then Sync Gradle (File -> Sync Project with Gradle Files)
