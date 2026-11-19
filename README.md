# DC Finance releases

Signed APKs of the DC Finance Android app, published as GitHub Release assets. Each release has:

- `dc-finance-<version>.apk`: the signed app (Digital Cookie key).
- `update.json`: `{versionCode, versionName, apkUrl, sha256, notes}`, read by the app's built-in updater.

The app checks `releases/latest`, downloads the APK, verifies its SHA-256 and that it is signed with the same key as
the installed app, then installs it. Nothing secret is in these files; sign-in happens in the app at runtime.
