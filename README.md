# Divolt Android

This is a fork of Revolt's Android TWA (Trusted Web Activity) for Divolt, a self-hosted instance of Revolt.

- [Get the latest APK](https://github.com/ggtylerr/divolt-android/releases/latest)
- ~~[Get it with F-droid](#)~~ (soon™) (probably™) (don't count on it though™)

## Build

~~Automatic builds are made with [GitHub Actions.](https://github.com/ggtylerr/divolt-android/actions)~~ Automatic builds are currently not done as GH Actions doesn't support prompts. Work is being done to fix this, but right now, all releases are manually built.

To manually build, you'll need the [Java 11.](https://adoptium.net/temurin/releases?version=11) Then generate `android.keystore`:

```sh
keytool -genkey -v -keystore android.keystore -alias android -keyalg RSA -keysize 2048 -validity 10000
```

You'll also need Bubblewrap: `npm i -g @bubblewrap/cli`

After you have it, and you can start building by doing `bubblewrap build`.
