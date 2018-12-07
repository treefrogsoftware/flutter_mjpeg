# flutter_mjpeg

This plugin provides MJPEG video streaming for Flutter. It uses [ipcam-view](https://github.com/niqdev/ipcam-view) library for Android part, and a custom implementation for iOS part.

This is just a proof-of-concept, rather than a full-fledged plugin. Pull requests are welcome.

## Getting Started

See the ```example``` for details.

When you try this plugin in your own app, the compiler will complain about duplicate value in ```AndroidManifest.xml```. Add the following to ```<application>``` tag of your ```AndroidManifest.xml```:

```
   tools:replace="android:label"
```

and also this to the top-most ```<manifest>``` tag:

```
    xmlns:tools="http://schemas.android.com/tools"
```

ipcam-view uses version 28 for the Android SDK.  With version 28 to avoid issues with URLs add the following to ```<application>``` tag of your ```AndroidManifest.xml```:
```
        android:usesCleartextTraffic="true"
```


