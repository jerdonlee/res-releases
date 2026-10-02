# Res releases

Public APK updates for **Res Owner** and **Res Subject**. Application source is maintained in the private res repository.

Download both apps from [the latest release](https://github.com/jerdonlee/res-releases/releases/latest):

- **Res Owner** (`com.res.owner`) goes on the controller phone.
- **Res Subject** (`com.res.subject`) goes on the supported phone.

Version 0.5.0 supplies the configured HTTPS/WSS relay in Subject. Create an invitation, pair by NFC or paste the manual invitation into Owner, and compare the matching code. Existing pairings keep their saved address; revoke and pair again to switch a local pairing to the public relay.

Owner supports screen viewing, taps, swipes and Back/Home/Recents after Subject approves Android screen sharing and enables Res touch control in Accessibility settings. Camera sessions support live viewing and MP4 recording. Subject can explicitly enable hands-free camera monitor with a visible Stop notification; permissions and saved pairing do not automatically restart capture after an interruption. Each new screen session still requires Android approval.

The relay runs on the project owner's Windows PC through a reserved secure tunnel. That PC must stay signed in, awake and online. Tunnel outages can interrupt sessions.

In either app, use **Settings → Update app** to check, download and install updates. Android asks for installation permission and confirms the update. Res verifies exact APK size, SHA-256, package, version and the installed signing certificate. **Try again** retries a failed download.

Older development APKs use Android Debug signing and need a one-time uninstall/reinstall to switch to release signing; pair again afterward. Later releases update in place. Installing an update stops sharing; enable Subject camera monitor again afterward.

Each release includes both signed APKs, latest.json and SHA256SUMS.txt. Downloads need no login. Signed APKs were tested on Android 16 and 17 emulators through the public relay. Physical NFC, camera behavior and manufacturer battery management still need device testing.
