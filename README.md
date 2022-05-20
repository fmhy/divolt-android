# Divolt Android

This is a fork of Revolt's Android TWA (Trusted Web Activity) for Divolt, a self-hosted instance of Revolt.

- [Get the latest APK](https://github.com/ggtylerr/divolt-android/releases/latest)
- ~~[Get it with F-droid](#)~~ (soon™) (probably™) (don't count on it though™)

## Build

Automatic builds are made with [GitHub Actions.](https://github.com/ggtylerr/divolt-android/actions)

To manually build, you'll need the `android.keystore`, and your own signing key:

```sh
keytool -genkey -v -keystore android.keystore -alias revolt -keyalg RSA -keysize 2048 -validity 10000
```

After you have it, and you can start building:

1. `yarn`
2. `yarn build`
