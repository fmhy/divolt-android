# Divolt Android

This is a fork of Revolt's Android TWA (Trusted Web Activity) for Divolt, a self-hosted instance of Revolt.

- [Get the latest APK](https://github.com/fmhy/divolt-android/releases/latest)
- [Get it with F-droid](https://fdroid.ggtyler.dev)

Alternatively, if you would prefer, you can install [RVMob](https://github.com/revoltchat/rvmob) and set apiURL to `https://api.divolt.xyz`, it is currently unfinished though.

## Build

~~Automatic builds are made with [GitHub Actions.](https://github.com/fmhy/divolt-android/actions)~~ Automatic builds are currently not done as GH Actions doesn't support prompts. Work is being done to fix this, but right now, all releases are manually built.

To manually build, you'll need the [Java 11.](https://adoptium.net/temurin/releases?version=11) Then generate `android.keystore`:

```sh
keytool -genkey -v -keystore android.keystore -alias android -keyalg RSA -keysize 2048 -validity 10000
```

You'll also need Bubblewrap: `npm i -g @bubblewrap/cli`

After you have it, and you can start building by doing `bubblewrap build`.

## Troubleshooting

If you're having problems, first try installing / updating `Android System Webview`(https://play.google.com/store/apps/details?id=com.google.android.webview), and if that doesn't work, then update your browser. Also, check if the problem you have occurs when you [go to the website in your browser.](https://divolt.xyz)

If all else fails, and it's not listed in the known bugs, please [report an issue](https://github.com/fmhy/divolt-android/issues) and let us know :)

## Known Bugs

None at the moment!
