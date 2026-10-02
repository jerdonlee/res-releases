# Res releases

Public APK updates for Res Owner and Res Subject. Application source is maintained separately in the private res repository.

Download the matching app from [the latest release](https://github.com/jerdonlee/res-releases/releases/latest):

- **Res Owner** (`com.res.owner`) goes on the controller phone.
- **Res Subject** (`com.res.subject`) goes on the supported phone.

In either app, open **Settings → Update app** to check, download and install updates. Android asks you to allow installation from Res and confirm the update. Res verifies the APK size, SHA-256, package, version and installed signing certificate before opening the installer. A failed download can be retried with **Try again**.

Older development APKs use Android Debug signing and require a one-time uninstall/reinstall to switch to these release-signed APKs; this removes local pairing and requires pairing again. Later releases from this channel can update in place. Installing an update stops active sharing; enable Subject camera monitor again afterward.

Each release includes the two signed APKs, latest.json update metadata and SHA256SUMS.txt. No login is needed for downloads. Pairing and internet sessions require a separately configured HTTPS relay; a public relay is not provided by this repository.
