# Project to reproduce issue resolving module in Metro

Command:

```
npm run bundle
```

Output:

```
> MetroBug@0.0.1 bundle /projectdir/MetroBug
> node node_modules/react-native/local-cli/cli.js bundle --entry-file index.js --platform android --dev false --reset-cache --bundle-output main.bundle

Scanning folders for symlinks in /projectdir/MetroBug/node_modules (22ms)
Scanning folders for symlinks in /projectdir/MetroBug/node_modules (18ms)
Loading dependency graph, done.
warning: the transform cache was reset.

Unable to resolve module `../../../../React` from `/projectdir/MetroBug/node_modules/react-native/Libraries/Components/ActivityIndicator/ActivityIndicator.js`: The module `../../../../React` could not be found from `/projectdir/MetroBug/node_modules/react-native/Libraries/Components/ActivityIndicator/ActivityIndicator.js`. Indeed, none of these files exist:

  * `/projectdir/MetroBug/node_modules/React(.native||.android.js|.native.js|.js|.android.json|.native.json|.json)`
  * `/projectdir/MetroBug/node_modules/React/index(.native||.android.js|.native.js|.js|.android.json|.native.json|.json)`
```